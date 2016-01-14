### meteorNginxDocker

container to download and configure nginx. It upgrades http connections to websockets.


### Important
#### SSL configuration.

Ensure to have your bundled certificate and ve generated the private key.

These two file must be stored within the `sslcerts` folder. It already contains 2 dummy files, replace them with your with theexact file names and extension. Reference the `README.md` file inside the `sslcerts` folder. 

#### nginx.conf
Replace `mydomain` with your domain. There are two places to do so.
This eonfiguration asserts that your meteor app is called `myapp`.


#### Installation

SSH into your server as super user

[Install docker.io](http://docs.aws.amazon.com/AmazonECS/latest/developerguide/docker-basics.html#install_docker) for the EC2 Ubuntu instance

###### commands
docker pull manminster/meteornginxdocke <br />
docker run -d manminster/meteornginxdocker tail -f /dev/null <br />
docker ps      (copy the ID) <br />
docker attach <ID> 
