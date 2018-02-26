FROM node:latest

# install git
RUN apt-get update && apt-get -y install git-core

# clone bts from github
RUN git clone https://github.com/phihag/bts.git

# open port
EXPOSE 4000

# run apache
RUN make -C ./bts
CMD cd /bts && /usr/bin/env node /bts/bts/bts.js


