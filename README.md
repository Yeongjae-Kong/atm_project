# ATM_project

### Requirements

2.1 System Setup
- (REQ1.1) An ATM has a serial number that can be uniquely identified among all ATMs.
- (REQ1.2) An ATM is set to one of the following types: (1) Single Bank ATM, (2) Multi-Bank ATM.
- (REQ1.3) An ATM may support either unilingual or bilingual languages.
- (REQ1.4) A Bank deposits a certain amount of cashes to an ATM to serve users.
- (REQ1.5) A Bank can open an Account for user with necessary information to perform bank services.
- (REQ1.6) A user may have multiple Accounts in a Bank.
- (REQ1.7) A user may have Accounts in multiple Banks.
- (REQ1.8) Each ATM have several types of transaction fees as follows
- (REQ1.9) An admin can access the menu of "Transaction History" via an admin card (See REQ Display of Transaction History).

2.2 ATM Session
- (REQ2.1) A session starts when a user inserts a card.
- (REQ2.2) A session ends whenever a user wishes (e.g., by choosing a cancel button) or there are some exceptional conditions detected by the ATM (e.g., no cash available).
- (REQ2.3) When a session ends, the summary of all transactions performed in a session must be displayed.
- (REQ2.4) Each transaction has a unique identifier across all sessions.

2.3 User Authorization
- (REQ3.1) An ATM checks if the inserted card is valid for the current type of ATM.
- (REQ3.2) If an invalid card is inserted, the ATM shall display an appropriate error message (e.g., Invalid Card).
- (REQ3.3) An ATM shall ask a user to enter the password (e.g., Enter Password), and verify if the password is correct
- (REQ3.4) If the entered password is incorrect, the ATM shall display an appropriate error message (e.g., Wrong Password).
- (REQ3.5) If a user enters wrong passwords 3 times in a row, a session is aborted, and return the card to the user.

2.4 Deposit
- (REQ4.1) An ATM shall take either cash or check from a user.
- (REQ4.2) An ATM shall display an appropriate error message if the number of the inserted cash or checks exceed the limit allowed by the ATM.
- (REQ4.3) Once cash or checks are accepted by ATM, the transaction must be reflected to the bank account as well (i.e., the same amount of fund must be added to the corresponding bank account).
- (REQ4.4) Some deposit fee may be charged (See REQ in System Setup)
- (REQ4.5) The deposited cash increase available cash in ATM that can be used by other users.
- (REQ4.6) The deposited check does not increase available cash in ATM that can be used by other users.

2.5 Withdrawal
- (REQ5.1) An ATM shall ask a user to enter the amount of fund to withdraw.
- (REQ5.2) An ATM shall display an appropriate error message if there is insufficient fund in the account or insufficient cash in the ATM.
- (REQ5.3) Once the withdrawal is successful, the transaction must be reflected to the bank account as well (i.e., the same amount of fund must be deducted from the corresponding bank account).
- (REQ5.4) Some withdrawal fee may be charged (See REQ in System Setup).
- (REQ5.5) The cash withdrawal lower available cash in the ATM that can be used by other users.

2.6 Transfer
- (REQ6.1) An ATM shall ask a user to choose the types of transfer either cash transfer or account fund transfer.
- (REQ6.2) For both cash and account transfers, an ATM shall ask the destination account number where the fund is to be transferred.
- (REQ6.3) For cash transfer, an ATM shall ask user to insert the cash, and verify if the amount of the inserted cash is correct.
- (REQ6.4) For account transfer, an ATM shall ask the source account number, and the amount of fund to be transferred.
- (REQ6.5) Some withdrawal fee may be charged (See REQ in System Setup).
- (REQ6.6) The inserted cash for transfer increase available cash in ATM that can be used by other users.
- (REQ6.7) Once the transfer is successful, the transaction must be reflected to the bank account as well (i.e., the same amount of fund must be deducted from the source bank account, and then added to the destination bank account).

2.7 Display of Transaction History (Admin Menu)
- (REQ7.1) When a session is started by an admin by inserting an admin card (See REQ in System Setup), an ATM displays a menu of "Transaction History" only.
- (REQ7.2) When the "Transaction History" menu is selected, an ATM display the information of all transactions from all users from the beginning of the system start
- (REQ7.3) The "Transaction History" information shall be outputted to the external file (e.g., txt file).

2.8 Multi-language support
- (REQ8.1) An ATM that is configured with the bilingual support shall provide an option for a user to choose the preferred language either English or Korean.
- (REQ8.2) Once a certain language is chosen, all menus must be displayed using the chosen language.
