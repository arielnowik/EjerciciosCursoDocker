FROM node:8
WORKDIR /usr/src/app
RUN git clone https://github.com/nicopaez/passwordapi /usr/src/app
RUN npm install --only production
EXPOSE 3000
CMD ["npm", "start"]