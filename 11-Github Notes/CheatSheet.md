- How to change from (main) to a new branch
- 0. Sync Fork repository
  1. `git checkout main`
  2. `git pull`
  3. `git checkout -b exampleBranchName`
- After I've written new code, These are the steps to save and add new changes back into main
  1. `git add .`
  2. `git status`
  3. `git commit -m "this section is to explain briefly a message of what i did"`
  4. `git push`- copy and paste terminal output
- New code will be pushed to GitHub but a pull request will need to be created.
- To create a pull request, these are the steps
  1. Go to forked repository and click on green banner (click compare and pull request)
  2. Add a description of what I completed
  3. Assign myself and a reviewer with tags
  4. After review has been made, squash and Merge
  5. After Merge is complete, switch back to main on VS code and sync fork reporitory on github browser
