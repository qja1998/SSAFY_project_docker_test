# frontend/Dockerfile
FROM node:14

WORKDIR /app

COPY package.json /app
# COPY package-lock.json /app

RUN npm install && npm audit fix

COPY . /app

# CMD [ "tail", "-f", "/dev/null" ]
CMD ["npm", "start"]