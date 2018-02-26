FROM node:latest

# install git
RUN apt-get update && apt-get -y install git-core

# clone bts from github
RUN git clone https://github.com/phihag/bup.git

# open port
EXPOSE 3001

# run apache
RUN npm install websocket
RUN npm install ws
RUN npm install node-webcrypto-ossl

CMD make root-hub -C ./bup
#RUN make -C ./bts
#CMD cd /bts && /usr/bin/env node /bts/bts/bts.js
