FROM alpine

WORKDIR /mydir 
RUN apk add --update \
    python \
    curl

RUN touch hello.txt 

RUN curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl 
RUN chmod a+x /usr/local/bin/youtube-dl 
ENV LC_ALL=C.UTF-8 
ENTRYPOINT ["/usr/local/bin/youtube-dl"] 
