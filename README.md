# jenkins-nginx

Deploy nginx with jenkins using docker-compose <br>
Step by step:
1. Build jenkins and nginx docker images <br>
```docker build -t [CONTAINER_NAME] .```
2. Run ```docker-compose up -d```
3. Create jenkins build
   - SCM Git: https://github.com/naufalrafih/jenkins-nginx
   - Branch Specifier: */main
   - Trigger: Poll SCM * * * * * (check every minute)
   - Add jenkins-build to execute shell
