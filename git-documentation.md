## Cheatsheet
This is a reference list of the most commonly used Git commands. (You might consider bookmarking this handy page.) Try to familiarize yourself with the commands so that you can eventually remember them all:

### Start your SSH agent
ssh -T git@github.com
    output: Enter passphrase for key '/Users/belfordj/.ssh/id_ed25519': bageatingLem0n

### Commands related to a remote repository:
git clone git@github.com:USER-NAME/REPOSITORY-NAME.git
git push or git push origin main (Both accomplish the same goal in this context)

### Commands related to the workflow:
git add .
git commit -m "A message describing what you have done to make this snapshot different"

### Commands related to checking status or log history
git status
git log

The basic Git syntax is program | action | destination.

For example,

git add . is read as git | add | ., where the period represents everything in the current directory;
git commit -m "message" is read as git | commit -m | "message"; and
git status is read as git | status | (no destination).

## Viewing your projects on the web
GitHub allows you to publish web projects directly from a GitHub repository. Doing this will allow you to access your project from your-github-username.github.io/your-github-repo-name.

There are a couple of ways to go about doing this, but the simplest is this:

make sure that the main HTML file of your project is called index.html. If it is not, you will need to rename it.
go to your GitHub repo on the web.
click on the Settings button from the panel at the top.
click on Pages on the left side bar.
change the Source from none to main branch and click Save.
it may take a few minutes (the GitHub website says up to 10, but we’ve seen it take up to an hour. Do not add a “theme” to your project, or you may have git conflicts, instead, be patient.) but your project should be accessible over the web from your-github-username.github.io/your-github-repo-name (obviously substituting your own details in the link).