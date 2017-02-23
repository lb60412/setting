
# gitlab setting
 - create rsa
 <pre>
 	$ ssh-keygen -t rsa -C "Email"
 	$ Enter file in which to save the key (/Users/lv/.ssh/id_rsa): /Users/lv/.ssh/id_rsa_gitlab
 </pre>
 
# gitHub setting
 - create rsa
 <pre>
 	$ ssh-keygen -t rsa -C "Email"
 	$ Enter file in which to save the key (/Users/lv/.ssh/id_rsa): /Users/lv/.ssh/id_rsa_github
 </pre>

# setting ssh config
	$ touch config

<pre>	
	#gitlab
Host gitlab.moji.com 
	HostName gitlab.moji.com 
	Port 20443
	IdentityFile ~/.ssh/id_rsa_gitlab

#github
Host github.com
        HostName github.com   
        Port 22
	IdentityFile ~/.ssh/id_rsa_github
</pre>

# testing 
	$ ssh -T git@gitlab.moji.com
	$ ssh -T git@github.com
	
	
---

# github add tag

```
$ git add .
$ git commit -m "new info"
$ git tag -a v0.0.9 -m "v0.0.9" 
$ git push origin master
$ git push origin --tag
```
	
