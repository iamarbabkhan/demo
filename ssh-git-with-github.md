## Git Setup

### How to generate ssh and connect with github

1. git config --global user.name "iamarbabkhan"
2. git config --global user.email "arbabkhan579@gmail.com"
3. ls -al ~/.ssh
4. ssh-keygen -t rsa -b 4096 -C "arbabkhan579@gmail.com"
5. eval "$(ssh-agent -s)"
6. ssh-add ~/.ssh/id_rsa
7. cat ~/.ssh/id_rsa.pub
8. copy the ssh key
9. ssh -T git@github.com
10. git clone git@github.com:iamarbabkhan/demo.git
11. cd repo
12. git add .
13. git commit -m "commit message"
14. git push origin main

### How to resume work using ssh with github
1. cd repository
2. git remote -v
3. git fetch --all
4. git pull origin master
5. ssh-add -l
6. ssh-add ~/.ssh/id_rsa 
