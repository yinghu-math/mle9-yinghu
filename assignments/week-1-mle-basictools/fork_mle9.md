## Goal: 
- At the end, you will have a local repo that linked to both `FourthBrain/MLE-9` and your own remote repo, such as `mle9-name`
- You can fetch from `fourthBrain/MLE-9`
- You can fetch from and push to your own repo `mle9-name`

## Steps 

- Create a new repo on GitHub, say `mle9-name`

- Clone your repo to local 
```bash 
git clone <url to your repo>
```

- add remote fourthBrain/MLE-9 to your repo, and name it `MLE9`
```bash 
git remote add MLE9 <FourthBrain/MLE-9_url> 
# you want to give this remote a different name other than 'origin', say `MLE9` 
# repo_url is the one shared by Milica 
```

- checkout the `main` branch of the remote mle9 and name the branch `mle9`
```bash
git checkout -b mle9 MLE9/main 
# git checkout -b <branch_name> <remote_name>/<remote_branch_name>
```

- finally you can merge your branch `mle9` branch to your `main` branch, which is tracking `origin/main`

```bash 
git checkout main  # make sure you are on the main branch  
git merge mle9 --allow-unrelated-histories 
```

Commit the changes and push to your own repo 
```bash
git add. 
git commit -m "message-here"
git push   # or git push origin main 
```

I think after this, we should be able to fetch info from both remotes using `git fetch --all`, update the `mle9` branch, merge to `main`, and push to `origin/main`. 