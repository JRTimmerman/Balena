FROM arm32v6/eclipse-mosquitto



# installing an editor
#USER root
#RUN apt-get update && apt-get install nano
#RUN apt-get install mosquitto mosquitto-clients

#USER node-red

#RUN npm install node-red-contrib-resinio
#RUN npm install node-red-dashboard
#RUN npm install node-red-contrib-credentials

# install node-red-admin which is needed if you want to created hashed password for the node-red editor.
# RUN sudo npm install -g --unsafe-perm node-red-admin

COPY ./mosquitto/mosquitto.conf /mosquitto/config/mosquitto.conf
COPY ./mosquitto/entrypoint.sh /entrypoint.sh
COPY ./mosquitto/passwd /mosquitto/config/passwd

#ENTRYPOINT ["sh", "/entrypoint.sh"]
#CMD ["mosquitto_passwd",  "-U",  "mosquitto/config/passwd"]
