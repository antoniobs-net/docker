# Building an app the Docker way

Just some example coded by Antonio Bueno <mail@antoniobs.net> powered by www.antoniobs.net

### Read me

Creating our first app + docker

### Donation

If you want: https://antoniobs.net/donaciones

### Code

Happy docking!

## Application containerization 

### 1) Creating docker file

```
sudo docker build --tag=demo-app .
```

### 2) View the new image

```
sudo docker image ls
```

### 3) Running the new app

```
sudo docker run -p 4000:80 demo-app
```

### 4) Open you browser and go to 

```
http://127.0.0.1:4000/
```

### Output:

```
Bienvenido World!
Equipo: fa2c01d6d7e2
# de visitas: Ups!, Redis no esta disponible!
```

Done! :-)

