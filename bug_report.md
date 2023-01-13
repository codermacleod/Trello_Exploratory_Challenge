# Probably the next best bug report in the world...

## Invalid emails are being accepted for sign-up. 

When signing up to Trello, and when we input an invalid email - such as 
'codermacleod@gmail.00', the email is accepted and a new account is created.

## Description
It appears as though the TLD(top-level domain) has not been configured in 
accordance with email formatting standards. 
We are able to input invalid alphanumeric sequences (such as 00,87,99) 
into the TLD.

Expected output:

A pop-up box informing the user that the email is invalid.

![Screenshot 2023-01-13 at 10 29 21](https://user-images.githubusercontent.com/73422077/212305031-329554f4-578f-4c31-b799-bea8efa55315.png)

Actual output:

No pop-up box shown and account is created, showing the following page:

![Screenshot 2023-01-13 at 11 00 07](https://user-images.githubusercontent.com/73422077/212304709-20d99274-7939-4d7e-b783-5946af685978.png)


## Steps to Reproduce

1- Click 'Sign-up for free'

![Screenshot 2023-01-13 at 10 57 31](https://user-images.githubusercontent.com/73422077/212304190-97077e96-1be3-498b-8e2f-299a25f0ee12.png)

2- Enter First Name as 'John'

3- Enter Last Name as 'Doe'

4- Enter Username as 'johndoe'

5- Click 'Next'

![Screenshot 2023-01-13 at 10 58 27](https://user-images.githubusercontent.com/73422077/212304372-8994ae38-a137-40de-813f-37e2986d7af5.png)

//next page

6- Enter email as 'johndoe@gmail.00' (ensure 00 and not oo)

7- Enter password 'blahblah' 

![Screenshot 2023-01-13 at 10 59 23](https://user-images.githubusercontent.com/73422077/212304553-7010ec81-a960-4256-8a01-d6f8fa58a422.png)

8- Click 'Sign-up' and ensure page is navigated to:

![Screenshot 2023-01-13 at 11 00 07](https://user-images.githubusercontent.com/73422077/212304709-20d99274-7939-4d7e-b783-5946af685978.png)

9- Confirm account creation by logging in and arriving at:

![Screenshot 2023-01-13 at 11 00 39](https://user-images.githubusercontent.com/73422077/212304813-d2190346-4556-49c2-bcd4-1bca13fe5725.png)

## Severity

High

## Priority

Medium
