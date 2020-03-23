<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="http://maratona.fullcycle.com.br/public/img/logo-maratona.png"/></a>
</p>

## Descrição

RabbitMQ usado entre os microserviços da Maratona FullCycle.

## Rodar a aplicação

#### Crie os containers com Docker

```bash
$ docker-compose up
```

#### Accesse a UI do RabbitMQ no browser

```
http://localhost:15672

User: admin
Password: admin
```

#### Criar as seguintes filas e bindings na exchange amqp.direct
```
Exchange: amqp.direct
micro-mapping/new-position   routing-key : mapping.new-position	
micro-mapping/orders-new     routing-key : orders.new
micro-orders/change-status   routing-key : orders.change-status
positions                    routing-key : orders.new
```

## Fizemos um vídeo no Youtube ensinando como rodar na prática os microserviços com Nest.js

[https://www.youtube.com/watch?v=MRk2Y_h2F-Q](https://www.youtube.com/watch?v=MRk2Y_h2F-Q)
