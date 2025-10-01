FROM node:18
WORKDIR  /depi-task/depi-task/k8s /t6
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3000
CMD ["npm", "start"]

