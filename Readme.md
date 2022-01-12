SSH keypair setup for GitHub (or GitHub/GitLab/BitBucket, etc, etc)
Create a repo.
Make sure there is at least one file in it (even just the README.md)

Generate a SSH key pair (private/public):
```
ssh-keygen -t rsa -C "your_email@example.com"

```

or even better:

```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

Copy the contet of your id rsa.pub file to git hub ssh key section...

>Settings > ssh and gpg keys
```

https://github.com/settings/keys
```

now check the authentication
Test the SSH key:
```

ssh -T git@github.com
```


Genral thing

how to push new repo

 create a new repository on the command line
 
 ```

echo "# namerepstry" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:yvenkets/name.git
git push -u origin main
```

push an existing repository from the command line

```
git remote add origin git@github.com:yvenkets/name.git
git branch -M main
git push -u origin main

```

