FROM lscr.io/linuxserver/transmission:latest

# Set environment variables
ENV PUID=1000
ENV PGID=1000
ENV TZ=Europe/Budapest

# Expose required ports
EXPOSE 9091
EXPOSE 51413
EXPOSE 51413/udp

# Set volume mounts
VOLUME /home/krsztn/torrents/config:/config
VOLUME /home/krsztn/torrents/downloads:/downloads
VOLUME /home/krsztn/torrents/watch:/watch

# Restart policy
CMD [--restart unless-stopped]

