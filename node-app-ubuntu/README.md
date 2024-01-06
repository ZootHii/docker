1  apt-get install
2  apt-get update
3  apt-get install curl -y
4  curl -SLO https://deb.nodesource.com/nsolid_setup_deb.sh
5  chmod 500 nsolid_setup_deb.sh
6  ./nsolid_setup_deb.sh 21
7  apt-get install nodejs -y
8  cd opt/
9  mkdir node-app
10 cd node-app/
11 node index.js

THESE STEPS ARE EQUIVALENT WHAT WE DO IN Dockerfile