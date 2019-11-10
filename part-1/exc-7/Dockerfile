FROM alpine
RUN apk --no-cache add curl
RUN apk --no-cache add bash
COPY curler.sh .
CMD  ["sh","curler.sh"]