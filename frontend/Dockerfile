FROM node:18-bullseye-slim

# Set environment variable for 
ENV NODE_OPTIONS=--openssl-legacy-provider

WORKDIR /app

COPY . ./
RUN yarn

EXPOSE 8080

ENV HOST=0.0.0.0
ENV PORT=8080

RUN yarn build

CMD [ "yarn", "start" ]