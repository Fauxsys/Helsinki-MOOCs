FROM node:10

EXPOSE 8000

RUN git clone https://github.com/docker-hy/backend-example-docker
WORKDIR backend-example-docker
RUN npm install

ENV FRONT_URL=http://localhost:5000

CMD ["npm", "start"]

# docker image build -t backend-exercise:12 . && docker container run -p 8000:8000 -v `pwd`/logs.txt:/backend-example-docker/logs.txt --name backend-example -d --rm backend-exercise:12