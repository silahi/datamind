# Utilisation d'une image ubuntu
FROM ubuntu:18.04

# Mise a jour et installation des paquets apache2
RUN apt-get update && apt-get install -y apache2 

# Copie tous les fichiers du répertoire courant vers le répertoire /var/www/html
COPY . /var/www/html

# Exposition du port 80
EXPOSE 80

#Execution de la commande une fois le conteneur demarré
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]


