## Support de virtualisation KVM
### 1. Ajoutez la clé GPG officielle Docker à votre système

```ruby
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

```
### 2. Ajoutez le dépôt Docker à la liste de vos dépôts
```shell
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```
### 3. Mettez à jour la liste des paquets 
```sql
sudo apt-get update

```
### 4. Installez Docker 
```csharp
sudo apt-get install docker-ce
```

### 4. Utiliser la commande docker sans **sudo**
```shell
sudo groupadd -f docker
sudo chown root:docker /var/run/docker.sock
sudo usermod -aG docker $USER
newgrp grp docker
sudo systemctl restart docker
```

### 6. Vérifiez que Docker est correctement installé et que la config est bien
```ruby
docker run hello-world
```




