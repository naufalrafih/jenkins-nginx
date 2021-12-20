# Jenkins-nginx

Deploy nginx with jenkins using docker-compose <br>
Step by step:
1. Build jenkins and nginx docker images
2. Run docker-compose.yaml
3. Create jenkins build
   - SCM Git: https://github.com/naufalrafih/jenkins-nginx
   - Branch Specifier: */main
   - Trigger: Poll SCM * * * * * (check every minute)
   - Add jenkins-build to execute shell
