
--to build image
docker build -t volumns:v2 .
-- to create container
docker run --name named-volumns-container -v feedback:/app/feedback --rm -p 3000:80 -d volumns:v2