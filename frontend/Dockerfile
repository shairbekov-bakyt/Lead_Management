FROM node

WORKDIR /app/frontend
COPY package.json /app/frontend
COPY . /app/frontend

RUN npm install
RUN npm install react-scripts

EXPOSE 3000
CMD ["npm", "start"]