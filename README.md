# docker-laravel
Este é um docker básico com ambiente de desenvolvimento para laravel com PHP 7.2, banco de dados Postgres e Servidor Apache

## Instruções de uso
- Inicialmente copie o ```.env-example``` e renomeie para ```.env```
- Execute o comando ```sudo docker-composer up -d```

Após o build concluído, os containers "levantarão" automaticamente  
Será possível visualizar o status do container pelo comando ```sudo docker ps```

## Acesso ao container php
Para acessar o container php e gerenciar os seus projetos utilize o seguinte comando:
- ```sudo docker-compose exec --user=laradock php7 bash```

## Acesso ao container postgres
Para acessar o container postgres e gerenciar os seus bancos de dados utilize o seguinte comando:
- ```sudo docker-compose postgres bash```

### Para acessar o postgres
- ```psql -U default -w```

Por padrão o usuário do postgres é:  
> user: default  
> password: secret