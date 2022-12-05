FROM node

WORKDIR /app

COPY package.json /app 

RUN npm install

COPY . /app

EXPOSE 80

#docker build -t sacgaikwad/docker-volumns .
#docker run -p 1234:80 -d --rm --name volumnsContainer sacgaikwad/docker-volumns:latest 
#--rm : to auto remove the container when it is stopped
#dback:/app/feedback -v "C:\Users\sacgaikwad\OneDrive - Fiserv Corp\Desktop\Learnings\Docker\data-volumes-01-starting-setup\:/app" -v /app/node_modules sacgaikwad/feeback-node:volumns
#PS C:\Users\sacgaikwad\OneDrive - Fiserv Corp\Desktop\Learnings\Docker\data-volumes-01-starting-setup> docker run -p 2100:80 -d --name volumnsContainer -v feedback:/app/feedback -v "C:\Users\sacgaikwad\OneDrive - Fiserv Corp\Desktop\Learnings\Docker\data-volumes-01-starting-setup\:/app" -v /app/node_modules sacgaikwad/feeback-node:volumns

CMD ["node","server.js"]