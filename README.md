Samples for PayPal-Payout
===========================
Using paypal rest api NPM package

Paypal Payout API: we can transfer money to multiple parties.



###  Prerequisites

- To run the application you need Node.js and Node packages manager installed.

``` 
npm install
```

###  Run 

- To run the payout api file on Node.js console

```
coffee payout/payout.coffee -n
```

###  Use of payout methods

- To make payment to mulitple parties, call Payout.create()

```CoffeeScript
##way to call Payout.create()
receivers = [
       {
         'amount': '0.99'
         'email': 'vijay.choudhary@cisinlabs.com'
       }
       {
         'amount': '1.0'
         'email': 'shirt-supplier-two@mail.com'
       }
       {
         'amount': '0.90'
         'email': 'shirt-supplier-three@mail.com'
       }
     ]
payoutObj = new Payout #create instance of Payout class
console.log payoutInst.create(receivers) #call the method to transfer money to multiple/single party
```

