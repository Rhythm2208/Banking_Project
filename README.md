# BankingProjectPYTHON
Simple command-line banking system implemented in Python. Below is a description of the key features and components of the project:

### Project Overview:

The project represents a basic banking system where users can perform various operations such as opening a new account, viewing account records, making withdrawals, making deposits, printing passbook entries, and printing ledger status.

### Functionality:

1. **Opening an Account (`Open_acc`):**
   - Users can input details such as account number, customer name, father's name, address, and opening balance to open a new account.
   - The account details are serialized and stored in a binary file (`master_file.dat`).

2. **Viewing Account Records (`view_rec`):**
   - Users can view the details of all accounts stored in the master file (`master_file.dat`).
   - The account details are deserialized and displayed on the console.

3. **Withdrawal (`withdrawl`):**
   - Users can withdraw money from their accounts.
   - The program checks the account balance and updates both the master file and a transaction file (`Trans_file.dat`).
   - Transaction details include the account number, date, withdrawal amount, transaction type 'W', and updated balance.

4. **Deposit (`deposit`):**
   - Users can deposit money into their accounts.
   - The program updates both the master file and the transaction file with the deposit amount and transaction details.

5. **Printing Passbook Entry (`pri_pass`):**
   - Users can print the passbook entry for a specific account.
   - Transaction details from the transaction file (`Trans_file.dat`) related to the account are deserialized and printed.

6. **Printing Ledger Status (`pri_ledg`):**
   - Users can print the ledger status, summarizing deposit information for all accounts.
   - The program reads the master file and prints the account number, customer name, and balance for each account.
   - The total deposit in the bank is calculated and displayed.

### File Handling:
   - The project uses two binary files (`master_file.dat` and `Trans_file.dat`) to store account details and transaction records.

### User Interaction:
   - The program interacts with users through a command-line interface, prompting for user inputs and providing feedback.

### Conclusion:
   - The project serves as a foundational example of a simple banking system, but for real-world use, it would require additional features, security measures, and user interface improvements.

