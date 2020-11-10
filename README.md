# Webapp wyświetlające godzinę w Lublinie, Nowym Yorku, Sydney

Aplikacja stworzona na serwerze `nginx`

## Jak utworzyć projekt

Wszystkie komenty są wywoływane z folderu z projektem
Rozmiar obrazu  dość duży (21,8MBytes). Można zastosować obraz alpine i busybox.


### Zainstaluj docker 
-[Docker](https://docs.docker.com/get-docker/)

### Utwórz obraz

```bash
docker build -t timeapp:v1 .
```

### Uruchom kontener

```bash
docker run -d -p 80:80 timeapp:v1
```

### Uruchom aplikacje 

Uruchom aplikację webową pod adresem [localhost](127.0.0.1:80)
lub wywołaj firefox z terminala
```bash
firefox 127.0.0.1:80
```
