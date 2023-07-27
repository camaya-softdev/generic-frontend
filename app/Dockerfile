FROM node:18.15.0

WORKDIR /app

COPY /app/generic-front/entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

ADD ./app/generic-front .


RUN npm i -g vite
RUN npm install --include=dev


ENTRYPOINT ["/entrypoint.sh"]



CMD ["npm", "run", "dev"]