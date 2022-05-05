# Stripe
Strip payments platform in python code

![An image of stripe the company.](stripe-for-wordpress.png)
------------------------------------------------------------

## Installation

You don't need this source code unless you want to modify the package. If you just want to use the package, just run: `pip install --upgrade stripe`

Install from source with: `python setup.py install`

## Requirements
Python 2.7+ or Python 3.4+ (PyPy supported)

## Usage

The library needs to be configured with your account's secret key which is available in your Stripe Dashboard. Set `stripe.api_key to its value`
```
import stripe
stripe.api_key = "sk_test_..."

# list customers
customers = stripe.Customer.list()

# print the first customer's email
print(customers.data[0].email)

# retrieve specific Customer
customer = stripe.Customer.retrieve("cus_123456789")

# print that customer's email
print(customer.email)
```
