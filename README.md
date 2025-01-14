# gitlab/gitlab-runner/regestry-gitlab
Instructions for launching gitlab, gitlab runner, regestry gitlab
## 1. clone repository
`git clone https://github.com/AqV-rs/gitlab-gitlab-runner.git`
## 2. Preparing the file structure:
`mkdir -p ./data/docker/gitlab/{var/opt/gitlab,var/log/gitlab,etc/gitlab-runner,var/run/docker.sock}`
## 3. Change .env
`vim .env`
You need to change the password, domain.
You can change the ports, if you need to change port 80, you need to change it in docker-compose
## 4. Start Docker-compose
`docker-compose up -d`
## 5. Registration runner
go to your gitlab domain `http://domain.com/admin/runners` \
click `New instance runner` \
click `Run untagged jobs`\
click `Create runner`\
use command `docker exec -it gitlab-runner gitlab-runner register` in terminal \
copy your url from step 1(gitlab) and paste in terminal \
copy your token from step 1(gitlab) and paste in terminal \
set the name of the runner \
select `shell` \
\
### gitlab/gitlab-runner/regestry-gitlab ready 

