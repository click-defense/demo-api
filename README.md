# TOR detector API

## Description

We want to have an API that allow us to detect if an IP comes from a TOR Network Node. 

## API endpoints

We only need a single endpoint:

**Request**

```
POST /tor-node
Content-Type: application/json

{
  "ip": "8.8.8.8"
}
```

**Response**

```json
{
  "torNetwork": true
}

```

## Sources

You can access to this URL's to get the lists of TOR Nodes:

* [TOR Project Exit Nodes List](https://check.torproject.org/torbulkexitlist)
* [dan.me.uk TOR Node List](https://www.dan.me.uk/tornodes)

## Requirements

* You should make a fork the repository we provide you and make a Pull Request once you finish.
* The API must be built to work on AWS Serverless infrastructure.
* We need to be able to deploy it easily on our AWS account.
* Code must be tested, and tests must run automatically.
* All your work must be documented:
	* How to run project
	* How to run tests
	* How to deploy project
	* Justify all your infrastructure decisions

## Evaluation criteria

This is a list of the principal criteria we will follow in order to evaluate this challenge:

1. The application works
2. The application can be deployed easily
3. The application has tests that can run locally
4. The code is clean and easy to understand
5. The documentation provided is enough to let others join the project easily

No item in this list is more important than any other. We will evaluate it as a whole.

## Extra points

Any improvement you add to this application will be welcome and evaluated too.

* Data persistence to avoid analyze same IP several times
* Keep lists updated with scheduled tasks
* Automations to simplify the bootstrap of the project 

