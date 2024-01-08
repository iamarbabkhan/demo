## Git Setup

### How to generate ssh and intergrate git with github

git config --global user.name "iamarbabkhan"
git config --global user.email "arbabkhan579@gmail.com
ls -al ~/.ssh
ssh-keygen -t rsa -b 4096 -C "arbabkhan579@gmail.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
cat ~/.ssh/id_rsa.pub
copy the ssh key
ssh -T git@github.com
yes
git clone git@github.com:iamarbabkhan/demo.git
