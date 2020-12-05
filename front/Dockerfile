# doodle:
#   usepad: true
#   internalPadUrl: "http://localhost:4200/"
#   externalPadUrl: "http://localhost:4200/"
#   # padApiKey: "19d89ca52bc0fa4f19d6325464d9d7a032649b9fa68c111514627081e2784b4a"
#   organizermail: "olivier.barais@gmail.com"
#   tmpfolder: "/tmp/excelFiles/font"
# angular:
#   datasource:
#     db-kind: mysql
#     username: root
#     password: ""
#     jdbc:
#       url: jdbc:mysql://localhost:3306/tlc?useUnicode=true&characterEncoding=utf8&useSSL=false&useLegacyDatetimeCode=false&createDatabaseIfNotExist=true&serverTimezone=Europe/Paris
#       driver: com.mysql.cj.jdbc.Driver
#   hibernate-orm:
#     database:
#       generation: update
#   mailer:
#     from: test@quarkus.io
# #    host: smtp.sendgrid.net
#     host: localhost
#     port: 2626
# #    port: 465
# #    ssl: true
# #    username: ""
# #    password: ""
#     mock: false

# This defines our starting point
FROM node:14.15.1

#Creation of directory
RUN mkdir /usr/src/app 

#use directory as workdir
WORKDIR /usr/src/app

#installation of angular cli
RUN npm install -g @angular/cli

#installation de module node
# RUN npm install

#copy our Angular application to our Docker instance
COPY . .

# #Lets test our Dockerfile by building it
# docker build -t testimage .
