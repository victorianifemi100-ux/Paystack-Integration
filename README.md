# Paystack

A fintech company that helps businesses accept and manage online/offline payments across Africa.

## Getting Started with Paystack

1. **Create your Paystack account**

   Create an account using your business information and set up your Paystack profile.

2. **Complete Business Verification**

   Submit the required business and compliance information based on your location and business type.

3. **Choose an Integration Method**

   After setting up your account, choose how you want to connect Paystack to your business:

   - **No-Code:** Use Paystack's ready-made payment tools without writing code
   - **Low-Code:** Use available integrations and plugins with minimal development work
   - **Pro-Code:** Use Paystack's APIs and SDKs to build a customised payment experience

### Pro-Code Integration

Developers can integrate Paystack into their application using the Paystack API. This allows them to build customised payment experiences and manage transactions programmatically.

'''
< http://api.paystack.co/transaction/initialize \
-H "Authorization: Bearer **YOUR_SECRET_KEY**" \
-H "Content-Type: application/json" \
-d '{email": "customer@email.com", "amount": 20000}' \
-X POST
'''

## **What it can be used for** ##

Paystack can be used to accept and manage online payments on websites and applications. After integrating Paystack, customers can select a product or service, make a payment, and receive confirmation when the transaction is completed.

### Payment Process ###
A typical Paystack payment process involves the following steps:
|
