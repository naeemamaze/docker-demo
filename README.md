# docker-demo
# push the codes using vs code terminal
# Step 1
git init
# Step 2 
git remote add origin https://github.com/naeemamaze/docker-web.git
# Step 3
git add .
# Step 4
git commit -m "My first commit"
# Step 5
git pull origin main
# Step 6
git push origin main
# Step 7
After puhsing the codes, it will be available in  git hub repository here that link: https://github.com/naeemamaze/docker-demo
# step 8
AWS console launch Ubuntu instance
<img width="843" alt="image" src="https://github.com/naeemamaze/docker-demo/assets/91151516/f8b30da4-ebc8-4557-80a3-92f484949e82">
# Step 9
Deploy jenkins on that server, create job in jenkins and build application and here list out all jobs for this process
<img width="945" alt="8_jenkinsoverview" src="https://github.com/naeemamaze/docker-demo/assets/91151516/7d078dce-45e8-42b0-b229-c12b1bcd693d">
# Step 10
Build pipeline of the application
<img width="938" alt="pipeline2" src="https://github.com/naeemamaze/docker-demo/assets/91151516/2feb7a42-0762-41d2-b868-5d78a42836d9">
# step 11
# Build node.js app with docker following commands
FROM jenkins/jenkins:lts
USER root

RUN mkdir -p /tmp/download && \
 curl -L https://download.docker.com/linux/static/stable/x86_64/docker-18.03.1-ce.tgz | tar -xz -C /tmp/download && \
 rm -rf /tmp/download/docker/dockerd && \
 mv /tmp/download/docker/docker* /usr/local/bin/ && \
 rm -rf /tmp/download && \
 groupadd -g 998 docker && \
 usermod -aG staff,docker jenkins

USER jenkins

# docker image url  
https://hub.docker.com/repository/docker/naeemamaze/docker-nodejs-demo
# image information check into docker hub
https://hub.docker.com/r/naeemamaze/docker-nodejs-demo
<img width="952" alt="image" src="https://github.com/naeemamaze/docker-demo/assets/91151516/e5c5b4ef-8e5b-4e6b-8c8b-077cc6769a26">
# step 12
Verify the docker pull request from ubuntu instance
<img width="944" alt="1_dockerpull" src="https://github.com/naeemamaze/docker-demo/assets/91151516/962e2b0b-91b5-48d8-95fa-edcc490fed0c">
# step 13
Verify the output using cli mode
<img width="844" alt="2_dockercheckingonserver" src="https://github.com/naeemamaze/docker-demo/assets/91151516/bfed189a-0df9-4c13-baea-455ffa84eca0">
# step 14
Verify the output using browser Sample web application
<img width="798" alt="3_sampleoutputhttp" src="https://github.com/naeemamaze/docker-demo/assets/91151516/c97b1c65-4bbe-42a5-9fbe-4ae68720296c">


















