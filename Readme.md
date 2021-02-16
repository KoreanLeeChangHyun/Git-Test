# Git initialization setting


## git download
You can download git from the website below  
URL: <a href="https://google.com" target="_blank">go do download link</a>  
 

## git config
Before initialization git, You have to set the git config  
Open your git bash, and enter the command below  
<pre>
 $ git config -- global user.name "YOUR_NICKNAME"  
 $ git config -- global user.email "YOUR_EMAIL" 
</pre>

#### Example:  
YOUR_NICKNAME = TonyStark  
YOUR_EMAIL    = <span>tony@gmail.com</span>  
<pre>
 $ git config -- global user.name TonyStark  
 $ git config -- global user.email tony@gmail.com  
</pre>

Notie: When wirte your nickname, there should be no space  
Tony Stark (x)  
TonyStark  (o)  


## SSH setting
### SSH private Key create
To access your remote git repository from your local repository, you need SSH key.  
You can make an SSH key with the below command.  
<pre>
$ ssh-keygen
</pre>

#### Result:
you can pass with enther (If you skip, entered below)  
ENTER_NEW_SSH_DIR = /home/schacon/.ssh/id_rsa  
ENTHER_SSH_PW     = None  
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



\* Reference: [git-doc-ssh](<https://git-scm.com/book/en/v2/Git-on-the-Server-Generating-Your-SSH-Public-Key>)
