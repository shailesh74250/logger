# logger
Logger - Producer produces logs into Queue, Consumer consumes logs from Queue

- Producer .env.example

      NODE_ENV=development
      LOGGER_TRANSPORTS=console,queue
      LOGGER_ALLOWED_LEVELS=info,error,warn,debug
      DB_DIALECT=postgres
      DB_HOST=localhost
      DB_PORT=5432
      DB_USERNAME=postgres
      DB_PASSWORD=postgres
      DB_DATABASE=azilen_nestjs
      RABBITMQ_URI=amqp://admin:admin123@localhost:5672
      RABBITMQ_QUEUE=cms-queue


- Consumer .env.example

      NODE_ENV=development
      LOGGER_TRANSPORTS=console,file
      LOGGER_ALLOWED_LEVELS=info,error,warn,debug
      
      DB_DIALECT=postgres
      DB_HOST=
      DB_PORT=5432
      DB_USERNAME=postgres
      DB_PASSWORD=postgres
      DB_DATABASE=azilen_nestjs
      
      # RabbitMQ username and password
      RABBITMQ_USERNAME=guest
      RABBITMQ_PASSWORD=guest
      RABBITMQ_HOST=localhost
      RABBITMQ_PORT=5672
      RABBITMQ_VHOST=/

