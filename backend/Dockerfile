FROM node:20
EXPOSE 8080
ENV DB_HOST=mysql
RUN useradd expense
RUN mkdir /app/server
RUN chown expense:expense /app/server
WORKDIR /app/server
COPY package.json .
COPY  *.js .
RUN npm install 
CMD [ "node","index.js" ]