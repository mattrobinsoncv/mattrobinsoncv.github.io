Attempting to get gh-pages working with Cloud9

I found this didn't work so well with my repo because of the naming convention (githup pages sets up a repo as username.github.io), so I used the command line in Cloud9 to set up instead :
git remote add origin https://github.com/mattrobinsoncv/mattrobinsoncv.github.io.git

I also found that I could Clone easily enough, but I wasn't able to commit the changes due to authenticaion failures.  Turns out you need to use the SSH URL (thanks Stack Overflow, again!) instead, like this :
git remote set-url origin git@github.com:mattrobinsoncv/mattrobinsoncv.github.io.git