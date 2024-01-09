#Imagem Base do para a nossa imagem
FROM nginx
#Diretório base onde onde o docker vais ser utilizado
WORKDIR /app

#Comandos que vão ser executados ao iniciarlizar o container
# a barra (\) serve como o +, ele permite cortar a linha
RUN apt-get update && \
apt-get install vim -y

COPY html /usr/share/nginx
#RUN apt-get install vim -y

