# bookmark-app

- Define the Problem
    - Need for a bookmarking app to save websites
    - initially use local storage, so account not needed
    - Add/Display/Removing Bookmarks
- Confirm inputs
    - (Required) Name/URL (required, user input)
        - MUST be provided (because we're not a browser) - cannot be null/empty
    - (Optional) Note/Description - to elaborate, help remind users what the site is
- Test cases:
    - should fail if Name/URL input empty (required attribute)
- Brainstorming (Think about and choose solution)
    - User form with two required inputs: Name and URL (MVP)
        - optional note input
    - Structured as object containing objects
- Runtime Analysis
    - Big-O Notation - Time/Space Complexity of solution
    - Becomes more of an issue with a greater number of items, but since this is dependent upon the user to add new items, shouldn't be a significant factor
- Coding
    - const Bookmarks = {}
    - add new Bookmark
        - bookmark.name
        - bookmark.url
        - bookmark.dateAdded
        - bookmark.note (default value of null unless user-defined)
- Testing/Debugging




Implementation/Expansion options:
- site title as default "placeholder" text - (more advanced coding, because ability to fetch the url and grab the title is needed)
- Folder/Organizing System
    - default save location (or option for last used if a bookmark was added less than an hour ago?)
    - User-Defined Categories ("folders")
- Sorting Options 
    - organize alphabetically by name
    - organize by date added
- Check if URL is a duplicate
- Use Class/Subclass functionality