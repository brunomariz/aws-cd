[![Update EC2 Repo](https://github.com/brunomariz/aws-cd/actions/workflows/ec2_pull.yml/badge.svg)](https://github.com/brunomariz/aws-cd/actions/workflows/ec2_pull.yml)

# aws-cd

Steps to automate deployment on EC2 instance by pulling changes automatically on push

- Create EC2 instance with .pem key
- Add pem to repo (Settings > Security > Secrets and Variables > Actions > New Repository Secret) and name it EC2_SECRET
- Add ssh host and user to repo in a similar way with names SSH_USER and SSH_HOST
- Create action (Actions > set up a workflow yourself) as in [ec2_pull.yml](.github/workflows/ec2_pull.yml)
