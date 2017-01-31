FROM node
RUN mkdir /code
WORKDIR /code
ADD . /code/
RUN npm i -g angular-cli@latest
RUN npm i -g typescript
RUN npm i -g tslint
RUN npm i -g protractor
RUN npm i
RUN webdriver-manager update
RUN ./node_modules/.bin/webdriver-manager update
EXPOSE 4200
CMD ng serve --host 0.0.0.0