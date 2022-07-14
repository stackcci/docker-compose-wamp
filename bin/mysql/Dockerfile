FROM mysql:8

RUN export myvar=$(docker logs mysqlcontainer 2>&1 | awk '/GENERATED ROOT PASSWORD/ {print $5}')
RUN echo $myvar