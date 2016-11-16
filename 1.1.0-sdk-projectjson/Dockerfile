FROM microsoft/dotnet:1.1.0-sdk-projectjson

# Install node-js and npm
RUN apt-get update -yqq \
    && apt-get install -yqq --no-install-recommends \
    nodejs-legacy npm \
    && rm -rf /var/lib/apt/lists/*

# Install global dependicies for node
RUN npm config set loglevel warn \
    && npm install -g --quiet bower gulp