# Block 18 Workshop: Writing Test Specifications

## Unit Tests

1. A Function called "multiplication" that returns the product of the two input numbers.

- Expect ***multiplication(1,2)*** to be a number
- Expect ***multiplication(1,2)*** to be equal to 2
- Expect ***multiplication(-5, 5)*** to be equal to -25
- Expect ***multiplication(3,"g")*** to be an error

2. A function called "concatOdds" takes two arrays of integers as arguments. It should return a single array that only contains the odd numbers, in ascending order, from both of the arrays.

- Example: ***concatOdds([3, 2, 1], [9, 1, 1, 1, 4, 15, -1])***
    - ... should result in ***[-1, 1, 3, 9, 15]***
- Expect ***concatOdds([c, a, a], [d, b, e])*** to be an error
- Expect ***concatOdds([3, 2, 1], [-1, 5, 11])*** to return ***[-1, 1, 3, 5, 11]***
- Expect ***concatOdds([4, 5, 5, 6, 7, 1], [-2, 3, 5, 7, 65])*** to return ***[1, 3, 5, 7, 65]***
- expect ***concatOdds([4, 2, 6], [10, 8, 2])*** to return an empty array

## Functional Tests

1. A shopping cart checkout feature that allows a user to check out as a guest (without an account), or as a logged-in user. They should be allowed to do either, but should be asked if they want to create an account or log in if they check out as a guest.

    ### Guest Checkout
    - There should be a prompt to ask if the user wants to create an account.
    - On this prompt there should be a path to create the account, where the user inputs their information. (i.e., contact info, mailing/billing address, credit card info)
    - There should be another option that takes the user back to the cart as a guest.
    - The guest should have to input all of their information during the checkout process.
    
    ### Account Holder Checkout
    - There should be prompt for the user to verify their information or payment method.
    - There should be the ability for the user to change their information and save it.

    ### Either Case
    - If checking out with an empty cart, there should be a prompt that pops up to prevent the user from checking out.