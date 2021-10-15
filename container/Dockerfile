FROM nodered/node-red

# Set work directory
WORKDIR /usr/src/node-red

# download extensions
RUN set -x; \
    npm install node-red-dashboard && \
    npm install node-red-node-base64 && \
    npm install node-red-contrib-opcua
