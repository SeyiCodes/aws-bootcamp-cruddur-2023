FROM node:16.18

ENV PORT=3000

COPY . /frontend-react-js
WORKDIR /frontend-react-js
RUN npm install

RUN apt-get update

RUN set -ex; \
    apt-get -y install --no-install-recommends \
        curl=7.64.0-4+deb10u1
        
EXPOSE ${PORT}
CMD ["npm", "start"]