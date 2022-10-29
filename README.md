# Git-Commit-Guard

Blocks commit if files contain the string "unpkg.com"

1. Copy/paste the git_hooks directory into your project root directory

2. Run this git command:
git config core.hooksPath git_hooks

3. Add this to package.json to run the above command automatically upon npm/yarn install:
"scripts": {
    "preinstall": "git config core.hooksPath git_hooks"
}
