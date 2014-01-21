Attempting to get gh-pages working with Cloud9

I intially found that the instructions for setting up a Project with a github repo at 

https://docs.c9.io/setting_up_github_workspace.html

I found this didn't work so well with my repo because of the naming convention (githup pages sets up a repo as username.github.io), so I used the command line in Cloud9 to set up instead :

git remote add origin https://github.com/mattrobinsoncv/mattrobinsoncv.github.io.git

I also found that I could Clone easily enough, but I wasn't able to commit the changes due to authentication failures.  Turns out you need to use the SSH URL (thanks Stack Overflow, again http://stackoverflow.com/questions/19918904/cloud9-git-push-fatal-authentication-failed!) instead, like this :

git remote set-url origin git@github.com:mattrobinsoncv/mattrobinsoncv.github.io.git