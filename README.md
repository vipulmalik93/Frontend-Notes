<!-- README file created -->
<!-- It will contains frontend entire notes  of javascript, react, html, css-->













<!-- ############################################################################################################ -->
# Coding-And-Dsa
<!--  -->
<!-- here coding and dsa files are in this repo -->
<!-- It contains questions and solutions -->
<!-- It contains all the required coding and dsa material t crack FAANG companies -->
<!-- It contains easy to hard questions of both coding and dsa -->
<!-- extra commit added -->
<!-- extra commit added from company laptop -->


<!-- commands -->
 cat .git/config  : it is used to see config file in .git 
 the .git file is invisible we can see  itby ls -a.
 we have to run it in project folder 
 after .git/config we ran in terminal it shows like this:

 admin@abcs-MacBook-Air Frontend-Notes % cat .git/config                                                                
[core]
        repositoryformatversion = 0
        filemode = true
        bare = false
        logallrefupdates = true
        ignorecase = true
        precomposeunicode = true
[remote "origin"]
        url = git@github.com-personal:vipulmalik93/Coding-And-Dsa.git     
        fetch = +refs/heads/*:refs/remotes/origin/*
[branch "main"]
        remote = origin
        merge = refs/heads/main
[pull]
        rebase = false

<!-- Explanation of above one -->
  1.   this url  -> git@github.com-personal:vipulmalik93/Coding-And-Dsa.git , check this url in your project by running   <!-- cat .git/config -->. The url mentioned here after running this command sees the Host in system  <!-- config file -->  what is host if it matches than it sees Hostname and contacts that host i.e github.com and than from IdentityFile which is the ssh key it than matches the ssh key there if key matches than authentication sets uo and if not matches than authentication fails.

  2. git@github.com:vipulmalik93/Frontend-Notes.git (Might Not Work):

         -> github.com is the actual hostname of GitHub.
         -> When SSH sees github.com, it looks for a Host github.com entry in your ~/.ssh/config file.
         -> If you don't have a Host github.com entry that specifically points to id_ed25519_personal, SSH will use its  default behavior.
         -> The default behavior is to try the SSH keys in your ~/.ssh directory in a certain order, or use the key that is specified by a generic Host * entry if one exists.
         -> In your case, this is likely to use your default SSH key, id_ed25519.
         -> If id_ed25519 is not registered with your personal GitHub account (vipulmalik93), GitHub will deny access, and the command will fail.
         -> Even if the repo was cloned using this url, the ssh key that is used for authentication is the deciding factor.


<!-- We can open system config by this command nano ~/.ssh/config -->
 <!-- and this will come in that file -->

    Host github.com-personal
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_ed25519_personal

<!-- we can set url of any repo like this:
git remote set-url origin git@github.com-personal:vipulmalik93/Coding-And-Dsa.git
 -->


 <!-- command: git remote -v  
  shows this at terminal when run at project folder
 -->
origin  git@github.com-personal:vipulmalik93/Coding-And-Dsa.git (fetch)
origin  git@github.com-personal:vipulmalik93/Coding-And-Dsa.git (push)

The output origin git@github.com-personal:vipulmalik93/Coding-And-Dsa.git (fetch) and origin git@github.com-personal:vipulmalik93/Coding-And-Dsa.git (push) is from the git remote -v command, and it tells you about the remote repository named "origin" associated with your local Git repository


<!-- always do in new repo after cloning is to set the url like this:
    git remote set-url origin git@github.com-personal:vipulmalik93/Coding-And-Dsa.git
 -->

 for Coding-And-Ds repo:   git remote set-url origin git@github.com-personal:vipulmalik93/Coding-And-Dsa.git
 for frontendNotes repo:  git remote set-url origin git@github.com-personal:vipulmalik93/frontendNotes.git

 the last part will change from th eurl with the repo name. Always set that url because only than you can have access to push in that otherwise if you don't set that than if you tries to push code there tha it will push to that repo which url is set here.


 <!-- Inside .md file styling -->
 # H1 - Main title
## H2 - Section title
### H3 - Sub-section

**bold text**

*italic text*

~~strikethrough~~

> This is a blockquote.
[Link text](https://example.com)
![Alt text](https://example.com/image.png)
---   horizontal divider
✅ :white_check_mark:
🚀 :rocket:
💡 :bulb:


`let`

```console.warn("hi)```


To view style in vs code: Cmd + Shift + V



