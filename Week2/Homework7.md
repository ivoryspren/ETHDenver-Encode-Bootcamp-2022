Homework 7
Adding more functionality to the Volcano Coin contract
1. We made a payment mapping, but we haven’t added all the functionality for it yet.
Write a function to view the payment records, specifying the user as an input.
What is the difference between doing this and making the mapping public ?
2. For the payments record mapping, create a function called recordPayment that
takes
1. the sender’s address,
2. the receiver’s address and
3. the amount
as an input, then creates a new payment record and adds the new record to the
user’s payment record.
3. Each time we make a transfer of tokens, we should call the this recordPayment
function to record the transfer.
