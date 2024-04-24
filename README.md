## what is amqp?
AMQP (Advanced Message Queuing Protocol) is an open standard application layer protocol for message-oriented middleware. The defining features of AMQP are message orientation, queuing, routing, reliability and security.

## what it means? guest:guest@localhost:5672 , what is the first quest, and what is the second guest, and what is localhost:5672 is for?
guest:guest@localhost:5672 is the default username:password@hostname:port for RabbitMQ. The first guest is the username, the second guest is the password, and localhost:5672 is the hostname and port.

## Simulation slow subscriber
![Simulation slow subscriber](/assets/img/ss1.png)
In my case the queued messages touched 25 messages, that means after we add 1 second delay on the subscriber, the subscriber will delay 1 second to receive the message from message broker.

## Reflection and Running at least three subscribers
![Subscriber POV](/assets/img/ss3.png)
![RabbirMQ POV](/assets/img/ss2.png)

Based on queued message chart, there are some improvement after running the publisher 5 times comparing to 1 subscriber when we run 3 subscribers. The queued message is not touched 25 messages anymore, it's only touched 15 messages. That means the subscriber is able to receive the message faster than before.