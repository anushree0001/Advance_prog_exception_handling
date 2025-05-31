# Advance_prog_exception_handling
Overview
The Rural Bank Account Management System (RBAMS) is a console based Java application developed to simulate basic banking services provided by the Rural Bank of Nepal (RBN) to citizens in remote areas. The system supports operations on Savings and Current accounts, with features like interest calculation, overdraft handling, and custom exception management.

Features
Supports two types of accounts:
- SavingsAccount: Accrues interest, no overdraft allowed.
- CurrentAccount: Allows overdraft up to a defined limit.
- Customer can have multiple accounts (aggregation).
- Implements core OOP concepts: abstraction, inheritance, encapsulation, and polymorphism.
- Custom exception handling (InsufficientBalanceException) for rule violations.
- Console-based menu-driven UI for easy interaction.

Class Design & OOP Concepts
1. BankAccount (Abstract Class)
Attributes: accountNumber, accountHolderName, balance
Abstract Methods: deposit(), withdraw()
Demonstrates abstraction.

2. SavingsAccount (Child of BankAccount)
Adds interestRate and addInterest() method.
Prevents overdraft withdrawal.
Demonstrates inheritance and polymorphism.

3. CurrentAccount (Child of BankAccount)
Adds overDraftLimit.
Allows withdrawal within overdraft limit.
Demonstrates inheritance.

4. Customer
Holds a list of BankAccount objects (aggregation).
Allows adding and displaying all associated accounts.
Demonstrates aggregation.

5. InsufficientBalanceException
Custom checked exception.
Thrown when withdrawal violates account constraints.
Demonstrates custom exception handling.

