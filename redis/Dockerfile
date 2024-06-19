# This temporary container will be used to issue the redis-cli command to the redis server

# Pull the official redis image
FROM redis:latest

# COPY [OPTIONS] <src>... <dest>
COPY ./entrypoint.sh /entrypoint.sh

# RUN <command> | 755: rwxr-xr-x 
RUN chmod 755 /entrypoint.sh

# ENTRYPOINT ["executable", "param1", "param2"]
ENTRYPOINT ["/entrypoint.sh"]