# GitHub Set-up Steps

### Git version control tool
Usually already installed on many Linux distros and macOS
https://git-scm.com/download
<br>

### Git Repositories
https://github.com
https://gitlab.com
https://bitbucket.org
<br>

### Create SSH key pair
https://help.github.com/en/articles/connecting-to-github-with-ssh
<br>

### Set Identity
If privacy settings for email are on, use private email address at https://github.com/settings/emails
```
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```
<br>

### Create a Repository
https://help.github.com/en/articles/create-a-repo
<br>

### Add Remote Repository
https://help.github.com/en/articles/adding-a-remote

https://help.github.com/en/articles/which-remote-url-should-i-use
<br>

### Managing Multiple Identities
Create new ssh key with a new name (examples below)
* id_rsa_a and id_rsa_b
* work_rsa and personal_rsa

To configure an individual repo to use a specific user / email address which overrides the global configuration. From the root of the repo run
```
git config user.name "Your Name Here"
git config user.email your@email.com
```

Create or modify config file
```
$ cd ~/.ssh/
$ touch config
$ subl -a config
```

Sample config file contents
```
#Personal GitHub account
Host github.com
 HostName github.com
 User git
 AddKeysToAgent yes
 UseKeychain yes
 IdentityFile ~/.ssh/id_rsa
 
#Work GitHub account
Host github.com-work
 HostName github.com
 User git
 AddKeysToAgent yes
 UseKeychain yes
 IdentityFile ~/.ssh/work_rsa
 ```
 
Use identity specified in config
* git clone git@github.com:personal/my_repo.git
* git clone git@github.com-work:[my work GitHub group]/[my project].git

### Markdown
* Default readme file format
* https://help.github.com/en/articles/basic-writing-and-formatting-syntax
* https://guides.github.com/features/mastering-markdown/