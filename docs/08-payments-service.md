# Microservices with Node JS and React [ENG, 2023]

<br/>

## Payments Service

<br/>

### Handling Payments

    $ cd payments
    $ npm install --save mongoose-update-if-current
    $ npm install --save stripe

<br/>

stripe.com

Developers --> API keys

<br/>

**Creating a Stripe Secret**

```
$ kubectl create secret generic stripe-secret --from-literal=STRIPE_KEY=<STRIPE_SECRET_KEY>
```

<br/>

    $ cd payments
    $ npm update @webmak/microservices-common

<br/>

Need to add <YOUR_STRIPE_PRIVATE_SECRET> for tests to file

<br/>

payments/src/test/setup.ts

<br/>

    $ npm run test

<br/>

```
Test Suites: 3 passed, 3 total
Tests:       8 passed, 8 total
Snapshots:   0 total
Time:        15.825 s
Ran all test suites.
```

<br/>