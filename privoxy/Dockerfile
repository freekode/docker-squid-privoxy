FROM ubuntu:bionic-20210222

RUN apt-get update && apt-get install -y privoxy wget
ADD privoxy-start.sh /usr/local/bin/
ADD config /etc/privoxy/
RUN chmod +r /etc/privoxy/config && chmod +x /usr/local/bin/privoxy-start.sh

EXPOSE 8118

CMD ["privoxy-start.sh"]
