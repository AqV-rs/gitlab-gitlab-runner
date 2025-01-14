# gitlab/gitlab-runner/regestry-gitlab
Instructions for launching gitlab, gitlab runner, regestry gitlab
## 1. clone repository
`git clone https://github.com/AqV-rs/gitlab-gitlab-runner.git`
## 2. Preparing the file structure:
`mkdir -p ./data/docker/gitlab/{var/opt/gitlab,var/log/gitlab,etc/gitlab-runner,var/run/docker.sock}`
## 3. Start Docker-compose
`docker-compose up -d`
## 4. 
