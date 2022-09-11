# Дефолтный конфиг nginx
<h4 align=center>
  <img alt=nginx src="https://www.nginx.com/wp-content/uploads/2021/08/NGINX-Part-of-F5-horiz-black-type-1.svg">
</h4>

> В данном репозитории находится дефолтный конфигурационный файл nginx.
> Этот репозиторий создан для проходения базового курса по ***GIT***  [`Devops by Rabrain`](https://rebrainme.com/devops/)

---

## Директивы

__nginx.conf__ содержит следующие основные директивы:
- location
- server
- server_name 
- listen
- root
- proxy_pass

## Пример

```javascript
server {
    location / {
        proxy_pass http://localhost:8080/;
    }
    location ~ \.(gif|jpg|png)$ {
        root /data/images;
    }
}
```

## Подробнее

Более подробно можно ознакомиться по ссылкам:
1. [`nginx.org`](https://nginx.org/ru/docs/beginners_guide.html)
2. [`highload.today`](https://highload.today/nginx/)

