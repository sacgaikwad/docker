
--to build image
docker build -t volumns:v3 .

-- to create container
docker run --name named-volumns-container -v feedback:/app/feedback -v "C:\Learn\Docker\Revision\docker\data-volumes-03-starting-setup\:/app" -v /app/node_modules -p --rm 3000:80 -d volumns:v3