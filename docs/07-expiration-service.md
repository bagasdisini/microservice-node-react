# Microservices with Node JS and React [ENG, 2023]

<br/>

## Expiration Service

<br/>

### Worker Services

<br/>

    $ cd expiration
    $ npm install --save bull @types/bull

<br/>

**push changes to github**

<br/>

    $ cd expiration
    $ npm update @webmak/microservices-common

<br/>

    $ cd orders
    $ npm update @webmak/microservices-common

<br/>

    $ cd orders
    $ npm run test

<br/>

```
// CREATE TICKET
// CREATE ORDER
```

<br/>

**After 15 minutes:**

```
[expiration] Event published to subject expiration:complete
[orders] Message received: expiration:complete / orders-service
[orders] Event published to subject order:cancelled
[tickets] Message received: order:cancelled / tickets-service
[tickets] Event published to subject ticket:updated
[orders] Message received: ticket:updated / orders-service
```

<br/>