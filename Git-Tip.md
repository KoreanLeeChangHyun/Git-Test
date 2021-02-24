# Git-tip

## Delete branch

Show branch list:
<pre>
  $ git branch
  $ git brnach -r
</pre>

Delete local branch: 
<pre>
  $ git branch -d <branch_name>
  $ git branch -r -d <branch_name>
</pre>

Delete remote branch:
<pre>
  $ git push origin --delete <branch_name>
</pre>

## Configration
Show configration
<pre>
  $ git config --list
</pre>

Set configration (email, nickname, defaultbranch)
<pre>
 $ git config -- global user.name 'YOUR_NICKNAME'  
 $ git config -- global user.email 'YOUR_EMAIL'
 $ git config -- global init.defaultBranch main
</pre>

## Log

Show log list
<pre>
  $ git log
  wq (out of log)
</pre> 

Save log to text file
<pre>
  $ git --no-pager log > log.txt
</pre>


