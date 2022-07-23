FROM node:16.13

WORKDIR /next

COPY package*.json ./
RUN yarn install
COPY . .

COPY startup.sh /startup.sh
RUN chmod 744 /startup.sh

EXPOSE 8080
CMD ["/startup.sh"]
