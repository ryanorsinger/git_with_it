## Now we know

- Frequently run `git status` to get your bearing.
- Before adding any files, you can use `git diff` to show change(s) to any un-staged file(s).
- Always use the SSH remote for GitHub and avoid the http.

## Troubleshooting
- We have to have commits to push. We have to have file(s) added in order to commit.
- Every commit requires a commit message.
- If we accidentally setup the remote as http, here's the fix:
	- `git remote -v` shows the remotes associated with your repository. 
	- If the remote shows https, we'll need to replace it with the ssh remote.
	- `git remote remove origin` to remove the old remote
	- Navigate to your repo in GitHub. Click the SSH button, then copy the git@github.com:username/repo_name.git link. This displays on the main page for an empty repository and is accessible under the green "Code" button if the repo already has content inside of it.
	- Once you've copied that git ssh address to your clipboard, go back to your terminal
	- type `git remote add origin`, a space character, and then paste the ssh address.
	- You have now reset your remote. To double check, do a `git push`
- If your ssh key is password protected and you don't need/want it to be, then follow these steps https://www.simplified.guide/ssh/set-remove-passphrase
- If you accidentally commited a sensitive file (or a file > 100mb), this video https://www.youtube.com/watch?v=liCAFV8Rmbs goes through how to remove that file from your git history (because deleting it is only a new fact on a permanent record machine)
- If you want to check and see if GitHub itself is experiencing problems, you can check https://www.githubstatus.com/
