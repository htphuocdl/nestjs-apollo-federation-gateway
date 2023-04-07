FROM node:18.15.0 AS BUILD_IMAGE

ENV CONTAINER_PATH=/home/app
WORKDIR $CONTAINER_PATH

RUN npm -v
RUN node -v

COPY ./ ./
RUN npm install --force
RUN npm run build

FROM node:18.15.0-alpine3.17

ENV CONTAINER_PATH=/home/app
WORKDIR $CONTAINER_PATH

# copy from build image
COPY --from=BUILD_IMAGE /home/app/dist ./dist
COPY --from=BUILD_IMAGE /home/app/package.json ./package.json
COPY --from=BUILD_IMAGE /home/app/src/app/domain/home/home.graphql ./graphql/home.graphql
RUN npm install --omit=dev --force

EXPOSE 3000 3000

ENTRYPOINT npm run start:prod