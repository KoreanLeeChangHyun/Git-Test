# Git initialization setting


## Git download
- You can download git from the website below  
  URL: <a href="https://google.com" target="_blank">go to download link</a>  
 

## Git Configuration
- Before initialization git, You have to set the git configuration  
  Open your git bash, and enter the command below  
<pre>
 $ git config -- global user.name 'YOUR_NICKNAME'  
 $ git config -- global user.email 'YOUR_EMAIL' 
</pre>

Example:  
- YOUR_NICKNAME = TonyStark  
  YOUR_EMAIL    = tony<spane>@</span>gmail.com  
<pre>
 $ git config -- global user.name TonyStark  
 $ git config -- global user.email tony@gmail.com 
</pre>

Note: When wirte your nickname, there should be no space  
- Tony Stark (x)  
  TonyStark  (o)  

\* Reference: https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration

## SSH setting
- To access your remote git repository from your local repository, you need SSH key.  
  You can make an SSH key with the below command.  
<pre>
$ ssh-keygen
</pre>

Result:
<pre>
Generating public/private rsa key pair.
Enter file in which to save the key (/home/schacon/.ssh/id_rsa): "ENTER_NEW_SSH_DIR"
Created directory '/home/schacon/.ssh'.
Enter passphrase (empty for no passphrase): "ENTHER_SSH_PW"
Enter same passphrase again: "ENTHER_SSH_PW"
Your identification has been saved in /home/schacon/.ssh/id_rsa.
Your public key has been saved in /home/schacon/.ssh/id_rsa.pub.
The key fingerprint is:
d0:82:24:8e:d7:f1:bb:9b:33:53:96:93:49:da:9b:e3 schacon@mylaptop.local
</pre>

Note: you can skip with enter (If you skip, entered below)  
- ENTER_NEW_SSH_DIR = /home/schacon/.ssh/id_rsa  
  ENTHER_SSH_PW     = None  

<pre>
$ cat ~/.ssh/id_rsa.pub
</pre>

Result:  
- Attach the key below to the GitHub SSH setup.
  GitHube -> setting -> SSH and GPG keys -> new SSH key -> attach your key  
<pre>
ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEAklOUpkDHrfHY17SbrmTIpNLTGK9Tjom/BWDSU
GPl+nafzlHDTYW7hdI4yZ5ew18JH4JW9jbhUFrviQzM7xlELEVf4h9lFX5QVkbPppSwg0cda3
Pbv7kOdJ/MTyBlWXFCR+HAo3FXRitBqxiX1nKhXpHAZsMciLq8V6RjsNAQwdsdMFvSlVK/7XA
t3FaoJoAsncM1Q9x5+3V0Ww68/eIFmb1zuUFljQJKprrX88XypNDvjYNby6vw/Pb0rwert/En
mZ+AW4OZPnTPI89ZPmVMLuayrD2cE86Z/il8b+gw3r3+1nKatmIkjn2so1d01QraTlMqVSsbx
NrRFi9wrf+M7Q== schacon@mylaptop.local
</pre>

Note: setting is 'profile setting' (not 'repository setting')  
- you can go 'profile setting' menu with enter the top bar user icon   

\* Reference: <https://git-scm.com/book/en/v2/Git-on-the-Server-Generating-Your-SSH-Public-Key>


## Git init

Create folder: 
- First make folder (this folder will become local repository)
  and open git bash  
<pre>
$ cd 'YOUR_FOLDER_DIR"
</pre>
Notice: You can replace with the below means (recommend)  
  Open your folder -> mouse right click -> git bash here  

Initialize local repository:
- You mush initialize your folder as the local repository.  
<pre>
$ git init
</pre>

\* Reference: https://git-scm.com/docs/git-init


## Git remote
- After initialize your local repository, you must connect your remote repository.  
  Githube -> your repositories -> new -> enter repository configuration -> create repository
  copy the 'SSH_URL' and attach
<pre>
  $ git remote add 'REPOSITORY_NAME' 'SSH_URL'
</pre>
  
Example:
<pre>
  git remote add origin git@github.com:username/repositoryname.git
</pre>

Note: recommend 'REPOSITORY_NAME' is 'origin'

\* Reference: <https://git-scm.com/book/en/v2/Git-on-the-Server-Generating-Your-SSH-Public-Key>


## Git fetch 

