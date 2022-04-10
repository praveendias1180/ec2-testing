# AWS EC2

# Protect Your Private Keys!

![Unprotected](unprotected.png)

# Connected to EC2 via SSH

![Connected](connected.png)

# Install NVM

```
curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash 

source ~/.bashrc

nvm install lts/* 

node -v

npm -v
```

# Install Git

```
sudo yum install git

git --version
```

# SSH Config

```
ssh-keygen -t ed25519 -C "praveendias1180@gmail.com"

ls -al ~/.ssh

eval "$(ssh-agent -s)"

ssh-add ~/.ssh/id_ed25519
```

![Keygen](keygen.png)

# Download and Add to Github

```
scp -i "aws-ec2.pem" ec2-user@ec2-3-141-8-44.us-east-2.compute.amazonaws.com:/home/ec2-user/.ssh/id_ed25519.pub /home/praveen/ec2

cat id_ed25519.pub
```
## Clone the repo, finally.

```
git clone git@github.com:praveendias1180/YOUR_REPO.git
```

# Bonus Packages

```
npm install -g serve
npm install -g pm2
```