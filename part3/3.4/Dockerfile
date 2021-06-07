FROM node:14.16-alpine

EXPOSE 5000

WORKDIR /usr/usr/app/

COPY . .

RUN npm install 
ENV REACT_APP_BACKEND_URL="http://localhost:8080/"
RUN npm run build && \
    npm install -g serve && \
    adduser --disabled-password appuser

USER appuser



CMD serve -s -l 5000 build