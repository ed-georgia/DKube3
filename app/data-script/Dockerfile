FROM alpine

RUN apk update && apk upgrade 
RUN apk add mysql-client

WORKDIR /opt

COPY import.sh /opt
COPY mydatabase.sql /opt


CMD [ "sh", "import.sh" ]  
