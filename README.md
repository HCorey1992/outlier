# outlier

# Clone the provided repository
git clone [URL of the provided repo]
cd [repo-name]

# Rebase base64 branch onto master
git checkout base64-branch
git rebase master

# Rebase user-agent branch onto master
git checkout user-agent-branch
git rebase master

# Merge rebased branches into master
git checkout master
git merge base64-branch
git merge user-agent-branch

# Set the new repo as origin and push changes
git remote set-url origin [URL of your new repo]
git push origin master
