## what is amqp?
AMQP (Advanced Message Queuing Protocol) is an open standard application layer protocol for message-oriented middleware. The defining features of AMQP are message orientation, queuing, routing, reliability and security.

## what it means? guest:guest@localhost:5672 , what is the first quest, and what is the second guest, and what is localhost:5672 is for?
guest:guest@localhost:5672 is the default username:password@hostname:port for RabbitMQ. The first guest is the username, the second guest is the password, and localhost:5672 is the hostname and port.

## Simulation slow subscriber
![Simulation slow subscriber](/assets/img/ss1.png)
In my case the queued messages touched 25 messages, that means after we add 1 second delay on the subscriber, the subscriber will delay 1 second to receive the message from message broker.