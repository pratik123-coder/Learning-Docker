# step 1 
FROM alpine

#step 2  : install a software 
RUN echo 'http://dl-cdn.alpinelinux.org/alpine/v3.6/main' >> /etc/apk/repositories
RUN echo 'http://dl-cdn.alpinelinux.org/alpine/v3.6/community' >> /etc/apk/repositories

RUN apk update 
RUN apk add mongodb=3.4.4-r0

#step 2.5 : Configure that software
VOLUME [ "/data/db" ]
WORKDIR /data
EXPOSE 27017

#step 3 : Set Default Command
CMD [ "mongod" ]


