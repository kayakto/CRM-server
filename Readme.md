```bash
    git clone https://github.com/kayakto/CRM-server.git project
```

```bash
    cd project
```

```bash
    mkdir -p nginx/certificates
```

```bash
    git clone https://github.com/kayakto/CRM-Module-Uralintern.git backend
```

```bash
    git clone https://github.com/vvvyat/crm.git frontend
```

```bash
    openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout nginx/certificates/bytebuilders-selfsigned.key -out nginx/certificates/bytebuilders-selfsigned.crt
```

```bash
    sudo docker-compose up --build -d
```