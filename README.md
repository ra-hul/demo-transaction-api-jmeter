# Transaction API With Jmeter

# About
This project demonstrates how to use JMeter for testing a transaction API. The steps tested include creating an agent and customer, 
depositing and withdrawing balance,checking balances, and making payments.

## Table of Contents

- [Test Scenarios](#test-scenarios)
- [Basic Info](#basic-info)
- [Steps for execute given scenarios](#steps-for-execute-given-scenarios)
- [Screenshot of html report](#screenshot-of-html-)


## Basic Info

 1. **baseUrl: dmoney.roadtocareer.net**
 2. **content-type: application/json**
 3. **constant timer:2000 milliseconds (which is used for create a delay between per request)**
 4. **Command for CLI to generate reports: jmeter -n -t Filename.jmx -l Filename.jtl -e -o Reports**

## Test Scenarios

The following test scenarios are implemented using JMeter:

1. **Admin creates an agent and a customer.**
2. **Deposit 2000 TK to agent from the system account (fromAc: SYSTEM).**
3. **Deposit 1000 TK to customer from agent account.**
4. **Check balance from customer account.**
5. **Withdraw 500 TK from customer account.**
6. **Payment of 200 TK from customer account (create any merchant acc or search for a merchant for payment).**


## Steps for execute given scenarios

The following steps are covered during design and execute the given scenarios

1. **Added a Thread Group under the test plan**
   
2. **Added HTTP Header Manager,User defined Variables,Constant Timer Under the thread group**
   
3. **Added HTTP Requests with POST Method,Those are: For Admin Login,For admin creates an agent,customer and merchant,To deposit to agent from system, deposit to customer from agent account,
   withdraw from customer account and payment to customer account**
  
4. **Added HTTP Request with GET Method to check customer balance**


## Screenshot of html report

![Jmeter_Assignment_part_2_Screenshot](https://github.com/ra-hul/demo-transaction-api-jmeter/assets/65038922/1363975e-cc44-4a69-8aa5-918193a5616d)
