# Bank Account Management System

This project demonstrates the use of C# List data structure to manage multiple bank accounts dynamically. It emphasizes the advantages of using C# List over other data structures for managing class objects.

## Project Overview

### Objective

The objective of this project is to:
1. Implement a `Bank` class that manages multiple `Account` objects using a C# List.
2. Provide functionalities to add accounts, execute transactions, and manage multiple accounts efficiently.

### Files Included

- `Program.cs`
- `Bank.cs`

### Instructions Followed

1. **Bank Class Implementation**:
    - **File**: `Bank.cs`
    - **Methods**:
        - `AddAccount`: Adds an account to the bank's list of accounts.
        - `GetAccount`: Retrieves an account by name from the bank's list of accounts.
        - `ExecuteTransaction`: Overloaded method to execute different types of transactions (`DepositTransaction`, `WithdrawTransaction`, `TransferTransaction`).

2. **Refactoring Main Program**:
    - **File**: `Program.cs`
    - **Enhancements**:
        - Added a new `Bank` object.
        - Implemented options for the user to create and manage accounts.
        - Refactored methods to use the `Bank` class for managing accounts and transactions.

### Key Features

- **Dynamic Account Management**: Utilize C# List to dynamically manage multiple bank accounts.
- **Method Overloading**: Implemented method overloading for `ExecuteTransaction` to handle different transaction types.
- **User Interaction**: Provides a user interface to create accounts, deposit, withdraw, and transfer money.

### How the Bank Class Works

1. **AddAccount Method**: Adds a new account to the bank's list.
2. **GetAccount Method**: Searches for an account by name and returns it. If no account is found, it returns `null`.
3. **ExecuteTransaction Method**: Executes the transaction passed as an argument.

### Demonstration

- **Creating an Account**:
    1. User is prompted to enter the account name and starting balance.
    2. A new `Account` object is created and added to the bank.
- **Depositing Money**:
    1. User selects the deposit option.
    2. User is prompted to enter the account name.
    3. The bank retrieves the account using `GetAccount`.
    4. User enters the deposit amount, and the transaction is executed.
- **Withdrawing Money**:
    1. Similar steps as depositing money.
    2. Ensure sufficient balance before completing the transaction.
- **Transferring Money**:
    1. User selects the transfer option.
    2. User is prompted to enter the source and destination account names.
    3. The bank retrieves both accounts and ensures neither is `null`.
    4. User enters the transfer amount, and the transaction is executed.

### Error Handling

- If an account cannot be found during any operation, an appropriate message is displayed to the user.

## How to Run the Program

1. **Compile the Program**:
    ```bash
    csc Program.cs Bank.cs
    ```
2. **Run the Program**:
    ```bash
    Program.exe
    ```

### Technologies Used

- `C#`
- `Visual Studio` or any C# compatible IDE

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


