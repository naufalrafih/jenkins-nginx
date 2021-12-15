# Jenkins-nginx

Deploy nginx with jenkins using docker-compose <br>
Step by step:
<ol>
  <li>Build jenkins and nginx docker images</li>
  <li>Run docker-compose.yaml</li>
  <li>Create jenkins build</li>
  <ul>
  <li>SCM Git: https://github.com/naufalrafih/jenkins-nginx </li>
  <li>Branch Specifier: */main</li>
  <li>Trigger: Poll SCM * * * * * (check every minute)</li>
  <li>Add jenkins-build to execute shell</li>
  <ul>
</ol>
