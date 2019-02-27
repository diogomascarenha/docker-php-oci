# Exemplo de PHP com OCI

## Criar a imagem
```
docker build --no-cache -t my-php-oci .
```

## Executar o container
```
docker run --rm -it --name my-php -v $(pwd):/app -w /app -u $(id -u):$(id -g) -p 8080:8080 my-php-oci php -S 0.0.0.0:8080
```

## Acessar no browser
```
http://127.0.0.1:8080/index.php
```

