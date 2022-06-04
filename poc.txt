FROM ubuntu

LABEL maintainer="sam@cognizantcompany.com"

RUN apt-get update && apt-get upgrade -y

RUN apt-get install nginx -y

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
