### Docker Practice 
* task 1 date 14.04.2023
* install docker usin linux vm
* login in terminal
* google docker install script
* using two commands 
* '''
* curl -fsSL https://get.docker.com -o get-docker.sh
# sh get-docker.sh
* '''
* do check docker --version
* docker info it shows no server
* we can add user 
* '''
* sudo usermod -aG docker 'username'
* '''
* ![preview](../images/dockerimage1.jpg)
* ![preview](../images/dockerimage2.jpg)
* check the docker images and also write down the size of hello-world
* ![preview](../images/dockerimage3.jpg)
* Run the nginx container with name as nginx and expose some port on docker host
* '''
* docker container run -d --name nginx1 -P nginx
* '''
* ![preview](../images/dockerimage4.jpg)
  ![preview](../images/dockerimage5.jpg)

* explain docker container lifcycle
* ---------------------------------
* docker life cycle state
* created
* running
* paused
* stopped
* deleted
* ![preview](../images/dockerimage6.jpg)
* docker architecture
* 