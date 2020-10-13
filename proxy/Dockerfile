FROM node: 12.18.3
ENV NODE_ENV=production
WORKDIR /proxy
COPY ["package.json", "package-lock.json*", "./"]
RUN npm install --production
EXPOSE 3004
COPY . .
CMD ["npm", "run", "start"]