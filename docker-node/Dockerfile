FROM node as builder
LABEL maintainer="teddy gauthier"

WORKDIR /node-app
COPY app.js .
COPY package.json .
RUN npm install

FROM node:16-alpine

WORKDIR /app
COPY --from=builder /node-app/app.js .
COPY --from=builder /node-app/node_modules node_modules
COPY --from=builder /node-app/package.json .
RUN adduser -D user
USER user

EXPOSE 3000

ENTRYPOINT ["node"]
CMD ["app.js"]
