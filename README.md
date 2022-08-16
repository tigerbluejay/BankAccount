# BankAccount
This console project defines two types, Account and Transactions. Transactions is a simple class that only holds information about transactions.

Account is class with three properties Number, Owner and Balance. Getting the balance recalculates it. The Account constructor defines an account number, sets the account owner and makes an initial balance deposit defined as a constructor parameter.

Account has three associated behaviors, MakeDeposit() creates a transaction and adds this transaction to the list of transactions defined as a private field in the Account class. MakeDeposit() throws an exception when and if deposit amount is not positive.

MakeWithdrawal() creates a transaction and adds it to the list of transactions defined as a private field in the Account class. And throws exceptions if amount of withdrawal is not positive and if there are not sufficient funds for this withdrawals.

GetAccountHistory() creates a stringbuilder to display account history, looping through the list of transactions.

Main() creates an account object, makes a withdrawal, recalculates the balance, makes a deposit, recalculates the balance and gets the account history.

Then we attempt to overdraw and the exception is caught. And we attempt to create an invalid account with negative balance, and the exception is caught.
