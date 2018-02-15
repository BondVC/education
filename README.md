# Welcome to Blockchain at Berkeley Developer's Decal site repository

## If you want to make changes to this repository please follow these steps.

1. [Install Hugo](https://gohugo.io/getting-started/installing/)
2. Clone the repo using the --recursive flag (git clone --recursive <project url>). If you don't use this tag you won't retrieve the website's theme, which is included as a git submodule.

Now switch into the repository directory. Run 'hugo server -D' to ensure the site is properly configured to be hosted locally. 

Once you've made the appropriate changes run 'hugo' to build the project. Then add, commit, and push your changes.

## How to properly make common edits

### Adding to the homepage's table

1. Copy the table in /content/_index.md
2. Navigate to https://www.tablesgenerator.com/markdown_tables
3. Select 'file >> Paste table data ...' and past the table from (1)
4. Add appropriate content in the table editor. Note the syntax for creating a linked item. Also, if multiple items are in the same table entry you must manually insert a <br/> between them.
5. Press 'generate' with 'Compact mode' selected
6. Replace the table in /content/_index.md with the newly generated markdown

## What you should not do

1. Make changes in the /themes/kube/ directory. This folder holds the default theme being used for this website and is setup as a git submodule. If you need to override some file (styling, partial, etc.) from the theme folder then duplicathe path to the file you want to override in the root directory of this repository. For example, if you want to override /themes/kube/static/css/custom.css (what you should do if you want to add custom css) then make changes to /statics/css/custom.css. 
