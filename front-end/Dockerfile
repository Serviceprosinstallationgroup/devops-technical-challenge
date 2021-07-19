FROM docker.io/library/node:alpine3.14
RUN node -v
COPY . .
RUN npm install parcel react-is

CMD ["npm", "start"]