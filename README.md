Samples for PayPal-Payout
===========================
using paypal rest api NPM package

Paypal Payout API: we can transfer money to multiple parties.


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
payoutInst = new Payout #create instance of Payout class
console.log payoutInst.create(receivers) #call the method to transfer money to multiple/single party
```




## Dependencies

``` 
npm install
```

Install Paypal rest api:
```
npm install paypal-rest-sdk --save

- To test the payout

```
node js/payout.js
```

or test directly: 
```
node test_payout.js
```
