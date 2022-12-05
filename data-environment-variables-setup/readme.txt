
--to build image
docker build -t volumns:v3 .

-- to create container
docker run --name env-variables-container -v feedback:/app/feedback -v "C:\Learn\Docker\Revision\docker\data-environment-variables-setup\:/app" -v named-volum:/app/node_modules --rm -p 3000:3001 --env-file environment.env -d env-variable:v1