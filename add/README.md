# add example
this folder contains an example of how to use the `git add` command

## change file

Open the git terminal in the this folder (add)

Use the `git status` command to make sure that there are no changes to the project. You should see "nothing to commit, working tree clean" written in the terminal

This folder contains a file called hipster.txt

Open hipster.txt in your prefered text editor and past the following paragraph below the one already there

"Offal sriracha farm-to-table, vice church-key neutra austin street art banjo unicorn seitan migas squid. Chillwave kitsch listicle shoreditch pug schlitz food truck, wolf tilde next level ennui pitchfork tote bag. Readymade 3 wolf moon chicharrones mixtape kickstarter try-hard listicle cold-pressed hashtag, echo park flannel. Try-hard asymmetrical artisan prism humblebrag kombucha farm-to-table enamel pin fingerstache venmo ennui semiotics cliche butcher raclette."

Now run the `git status` command again. The following message should appear in the terminal:

```On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   hipster.txt

no changes added to commit (use "git add" and/or "git commit -a")```

This message tells you that on your master branch (`origin/master`) there are new changes (`modified:   hipster.txt`) not added to the staging area (`Changes not staged for commit:`) i.e. these changes are still just in the working directory. In order to add these files to the staging area you have to use the `git add hipster.txt` command.

Once you have done this, run git `status again`. You will see the following confirming that the file is now in the staging area: 

```On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   hipster.txt
```