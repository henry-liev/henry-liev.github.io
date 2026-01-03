# Blog Directory

Place your markdown (.md) files in this directory.

## To add a new blog post:

1. Create a `.md` file in this directory (e.g., `2025-01-15-my-post.md`)
2. Add an entry to `posts.json` under the appropriate category with:
   - `filename`: the name of your .md file
   - `title`: the display title
   - `date`: the publication date (optional)

## Category Structure

Posts are organized by categories in `posts.json`. Each category is a key in the JSON object, and its value is an array of posts.

Example structure in `posts.json`:
```json
{
    "music": [
        {
            "filename": "top10albums2025.md",
            "title": "Top 10 Albums of 2025",
            "date": "January 1, 2026"
        }
    ],
    "thoughts": [
        {
            "filename": "my-thoughts.md",
            "title": "My Thoughts",
            "date": "January 15, 2025"
        }
    ]
}
```

## Adding Categories

To add a new category:
1. Add a new key to `posts.json` with an empty array: `"newCategory": []`
2. Add posts to that category's array
3. Categories are displayed in the order they appear in `posts.json` (first category is expanded by default)

## Notes

- The `date` field is optional - posts without dates won't display a date
- Posts within each category are displayed in the order they appear in the array
- Categories appear as collapsible dropdown menus on the blog page
