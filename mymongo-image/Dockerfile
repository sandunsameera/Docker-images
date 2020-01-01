#step 1
FROM alpine
#step 2:install a software
RUN echo 'http://dl-cdn.alphinelinux.org/alphine/v3.6/main' >> /etc/apk/repositories

RUN echo 'http://dl-cdn.alphinelinux.org/alphine/v3.6/commiunity' >> /etc/apk/repositories

RUN apk update
RUN apk add mongo=3.4.4-r0
#step 2.5:Configure the software

VOLUME [ "/data/db" ]
WORKDIR /data
EXPOSE 27017

#step 3:set defaulf command
CMD [ "mongod" ]


