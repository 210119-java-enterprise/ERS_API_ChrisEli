# Expense Reimbursement System
The Expense Reimbursement System (ERS) will manage the process of reimbursing employees for expenses incurred while on company time. All employees in the company can login and submit requests for reimbursement and view their past tickets and pending requests. Finance managers can log in and view all reimbursement requests and past history for all employees in the company. Finance managers are authorized to approve and deny requests for expense reimbursement.

## Technologies Used
* Java
* PostgreSQL
* AWS RDS
* Elastic Beanstalk
* AWS CodePipeline
* Postman
* Hibernate
* Servlets

## Features
- Exposed endpoints in a RESTful manner using Java servlets to support basic operations as defined by requirements documents
- Sends error message objects when requests cannot be processed
- Has logging
- Encrypts user passwords prior to persisting to data source
- Uses Hibernate
- Uses custom exceptions to replace generic RuntimeException instances
- Admins can add, remove, and adjust user accounts
- Users can submit, view and adjust reimbursements
- Financial managers can view and approve or dispprove reimbursement requests

## Getting Started
To use on AWS, fork project into github repo under your control. Using that fork, set up a AWS CodePipeline to Elastic Beanstalk. This will begin running the project.

## Usage
Endpoints are /Users, /Authentication and /Reimbursements. Authentication end point only takes get requests, and the connected server will require some initial accounts.
/Users can only be accessed by users who are logged in as an admin. The /reimbursements endpoint can be accessed by employees or Financial Managers. Employees can use this endpoint to view, change, and submit reimbursement request. Financial managers can view, change, and approve or deny reimbursement requests.

## Contributors
* Chris Nichols

## Docs
https://docs.google.com/document/d/1a8xoQ4vBYrwAbNLNN10U47VOeQAZPuhiiivBbLAWEC4/edit?usp=sharing
