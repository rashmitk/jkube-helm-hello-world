# springboot-hello-world
A simple helloworld microservice developed using SpringBoot

<pre>
Here are the supported resources to access the helloworld service :
  http://HOST:PORT:8084/
  http://HOST:PORT:8084/hello
  http://HOST:PORT:8084/hello/{message}
</pre>

mvn clean package k8s:build k8s:resource k8s:helm -Pkubernetes


Create a file inside ~/.m2/settings.xml with below config

<servers>
  <server>
    <id>docker.io</id>
    <username>DOCKER_LOGIN_USERNAME</username>
    <password>DOCKER_LOGIN_PASSWORD</password>
  </server>
  <!-- ... -->
</servers>
