# FROM node:13.1-alpine
# RUN mkdir -p /srv/app
# WORKDIR /srv/app/client
# ADD client /srv/app/client
# RUN  npm install


# CMD [“npm”, “start”]


# FROM mhart/alpine-node:11 AS builder
# WORKDIR /srv/app/client
# COPY . /srv/app/client
# RUN npm run start
# RUN ls -la

# FROM mhart/alpine-node
# RUN npm install -g serve
# WORKDIR /app
# COPY --from=builder /app/build .
# CMD ["serve", "-p", "80", "-s", "."]

FROM mhart/alpine-node
WORKDIR /srv/app/client
COPY . /srv/app/client
RUN npm install && npm install -g serve
CMD ["npm", "start"]
