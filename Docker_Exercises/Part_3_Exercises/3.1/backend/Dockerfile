FROM node:10

EXPOSE 8000

WORKDIR app

RUN git clone https://github.com/docker-hy/backend-example-docker && \
    npm install backend-example-docker && \
    rm -rf backend-example-docker

CMD ["npm", "start"]

# docker image build -t backend-exercise:3.1 . && docker container run -p 8000:8000 -v `pwd`/logs.txt:/backend-example-docker/logs.txt --name backend-example -d --rm backend-exercise:3.1