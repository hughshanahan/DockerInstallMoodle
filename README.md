This is a brief description of how to install a basic version of moodle locally.

- If you haven't done so, install [docker](https://www.docker.com/) on your computer. If you are using docker for the first time you will need to set your self up with an account on it (or else you cannot access docker hub and the next steps will generate an error message).

- With docker installed and running on your computer you can install the moodle container which is explained in detail [here](https://github.com/bitnami/bitnami-docker-moodle). There is a great deal on information there about how to configure it with passwords etc. but I'll just leave the default.  

- Go to a suitable directory and from your command line type 

  ```sh
  curl -sSL https://raw.githubusercontent.com/bitnami/bitnami-docker-moodle/master/docker-compose.yml > docker-compose.yml
  ```

  then

  ```sh
  docker-compose up -d
  ```

   With this second command moodle is now running on your computer.

  You can access the moodle page by going to a browser and typing 

  `http://localhost:80`

  You can then log yourself in with username `user` and password `bitnami` (all of this can be configured if you do a manual install with docker as outlined on the bitnami site.)

  

  
