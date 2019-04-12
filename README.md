# Mini Project

Hello! Thank you for taking the time to complete this project.

## Technical context:

Our services are delivered on a multi tenant high volume SaaS platform build on a micro service architecture.

The platform is primarily API driven. Clients access the platform via direct API, SFTP file transfers and via web UI.

All APIs are [JSONAPI](jsonapi.org) conformant implementing a standard RESTful interface.

The web UI is built on Angular. The platform is deployed on Kubernetes.

As with any complex application, consistent implementations, DRY code and reusability is critically important.

[SOLID](https://en.wikipedia.org/wiki/SOLID) design principles and TDD are also very important

As this is a platform serving multiple clients, code needs to make as few assumptions as possible.

Methods should be very flexible in their implementation and chaining them should be intuitive, for example A/R scopes

## Business context

The platform offers clients the ability to create rewards for their end users based on transactions the user conducts on the platform
A simple use case is:
1. For every $100 the end user spends they receive 10 points
2. If the customer accumulates 100 points in one calendar month they are given a reward, a free coffee
3. If the customer spends any amount of money in a foreign country they receive 2x the standard points

## Basic Requirements

A hypothetical client has the following requirements:

1. A gold tier customer is an end user who accumulates 1000 points or more in a calendar year
2. A platinum tier customer is an end user who accumulates 5000 points or more in a calendar year
3. Everyone else is a standard tier customer
4. For every $100 the end user spends they receive 10 points
5. If the customer accumulates 100 points in one calendar month they are given a reward, a free coffee
6. If the customer spends any amount of money in a foreign country they receive 2x the standard points

## Extended Requirements

1. Give a 4x Airport Lounge Access Reward when a user becomes a gold tier customer
2. Create a free coffee reward to all users during their birthday month

## Your Task

Implement an RoR based solution that implements the <b>Basic Requirements</b>. Your code should follow RoR current best practices
taking into account the technical context described at the top of this document. For example, given that it is a high volume environment, ensuring
data integrity is paramount. Appropriate tests are necessary. That kind of thing.

Use seed files to create users, tiers, transactions and rewards. It should be possible to run `rails db:seed` and have all the use cases manifest

If you need to do research, include a comment in the code with a URL to the document you referenced.
Not an exhaustive list, just include a single reference.
If you feel that explaining a design choice would help clarify the chosen solution please indclude comments in the code.

## Bonus Tasks

It is enough to build out the application, but if you feel inclined, we would be happy to see any or all of the following:

1. Implementation of the Extended Requirements
2. Implementation of a basic SDK that interfaces with the API
3. Postman collection that interacts with the API
4. Basic angular app that consumes the API
5. Terraform code that deploys a cloud instance running the application

None of these are a requirement and if you don't do them <b>it will not reflect in any way on the evaluation.</b>

## Finally

The primary purpose of this project is to help us better understand how you approach business requirements in code
and ultimately determine if we are a good fit for you and vice versa. We operate in a demanding environement where there is no shortage of
interesting and challenging work. It can be very satisfying, but first and foremost, we don't want to set anyone up for failure. We want you
to succeed and grow in your job and career, but we need to know that you have the experience and skills to meet the challenge on day 1.

Thank you again for your time. Clarifying questions are encouraged.
