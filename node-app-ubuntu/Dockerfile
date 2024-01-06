# docker pull ubuntu
FROM ubuntu
RUN apt-get update
RUN apt-get install curl -y
RUN curl -SLO https://deb.nodesource.com/nsolid_setup_deb.sh
RUN chmod 500 nsolid_setup_deb.sh
RUN ./nsolid_setup_deb.sh 21
RUN apt-get install nodejs -y

# // copy . ( . means everything (index.js will be copied)) from this folder to /opt/node-app/
# COPY . /opt/node-app/

# // command = CMD (this step can work but we can do better)
# CMD ["node", "/opt/node-app/index.js"]

# // or change workdir
# // workdir command changes working directory
WORKDIR /opt/node-app/
# // copy . (everything in local path which is have index.js) from this local path to ubuntu current workdir (we have changed it above /opt/node-app/) 
COPY . .
ENV whoami=zoothii
CMD ["node", "index.js"]

# THESE STEPS ARE EQUIVALENT WHAT WE DO on ubuntu in docker engine
