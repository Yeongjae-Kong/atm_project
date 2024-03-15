# atm_project

#### requirements

2.1 System Setup
w	(REQ1.1) An ATM has a serial number that can be uniquely identified among all ATMs. 
w	(REQ1.2) An ATM is set to one of the following types: (1) Single Bank ATM, (2) Multi-Bank ATM. 
w	(REQ1.3) An ATM may support either unilingual or bilingual languages. 
w	(REQ1.4) A Bank deposits a certain amount of cashes to an ATM to serve users.
w	(REQ1.5) A Bank can open an Account for user with necessary information to perform bank services. 
w	(REQ1.6) A user may have multiple Accounts in a Bank.
w	(REQ1.7) A user may have Accounts in multiple Banks.
w	(REQ1.8) Each ATM have several types of transaction fees as follows 
w	(REQ1.9) An admin can access the menu of “Transaction History” via an admin card (See REQ Display of Transaction History). 

2.2 ATM Session
w	(REQ2.1) A session starts when a user inserts a card.
w	(REQ2.2) A session ends whenever a user wishes (e.g., by choosing a cancel button) or there are some exceptional conditions detected by the ATM (e.g., no cash available). 
w	(REQ2.3) When a session ends, the summary of all transactions performed in a session must be displayed. 
w	(REQ2.4) Each transaction has a unique identifier across all sessions. 

2.3 User Authorization
w	(REQ3.1) An ATM checks if the inserted card is valid for the current type of ATM. 
w	(REQ3.2) If an invalid card is inserted, the ATM shall display an appropriate error message (e.g., Invalid Card). 
w	(REQ3.3) An ATM shall ask a user to enter the password (e.g., Enter Password), and verify if the password is correct 
w	(REQ3.4) If the entered password is incorrect, the ATM shall display an appropriate error message (e.g., Wrong Password). 
w	(REQ3.5) If a user enters wrong passwords 3 times in a row, a session is aborted, and return the card to the user. 

2.4 Deposit
w	(REQ4.1) An ATM shall take either cash or check from a user.
w	(REQ4.2) An ATM shall display an appropriate error message if the number of the inserted cash or checks exceed the limit allowed by the ATM. 
w	(REQ4.3) Once cash or checks are accepted by ATM, the transaction must be reflected to the bank account as well (i.e., the same amount of fund must be added to the corresponding bank account). 
w	(REQ4.4) Some deposit fee may be charged (See REQ in System Setup) 
w	(REQ4.5) The deposited cash increase available cash in ATM that can be used by other users. 
w	(REQ4.6) The deposited check does not increase available cash in ATM that can be used by other users. 
2.5 Withdrawal
w	(REQ5.1) An ATM shall ask a user to enter the amount of fund to withdraw. 
w	(REQ5.2) An ATM shall display an appropriate error message if there is insufficient fund in the account or insufficient cash in the ATM. 
w	(REQ5.3) Once the withdrawal is successful, the transaction must be reflected to the bank account as well (i.e., the same amount of fund must be deducted from the corresponding bank account). 
w	(REQ5.4) Some withdrawal fee may be charged (See REQ in System Setup).
w	(REQ5.5) The cash withdrawal lower available cash in the ATM that can be used by other users. 

2.6 Transfer
w	(REQ6.1) An ATM shall ask a user to choose the types of transfer either cash transfer or account fund transfer. 
w	(REQ6.2) For both cash and account transfers, an ATM shall ask the destination account number where the fund is to be transferred. 
w	(REQ6.3) For cash transfer, an ATM shall ask user to insert the cash, and verify if the amount of the inserted cash is correct. 
w	(REQ6.4) For account transfer, an ATM shall ask the source account number, and the amount of fund to be transferred. 
w	(REQ6.5) Some withdrawal fee may be charged (See REQ in System Setup).
w	(REQ6.6) The inserted cash for transfer increase available cash in ATM that can be used by other users. 
w	(REQ6.7) Once the transfer is successful, the transaction must be reflected to the bank account as well (i.e., the same amount of fund must be deducted from the source bank account, and then added to the destination bank account). 

2.7 Display of Transaction History (Admin Menu)
w	(REQ7.1) When a session is started by an admin by inserting an admin card (See REQ in System Setup), an ATM displays a menu of “Transaction History” only. 
w	(REQ7.2) When the “Transaction History” menu is selected, an ATM display the information of all transactions from all users from the beginning of the system start 
w	(REQ7.3) The “Transaction History” information shall be outputted to the external file (e.g., txt file). 

2.8 Multi-language support
w	(REQ8.1) An ATM that is configured with the bilingual support shall provide an option for a user to choose the preferred language either English or Korean. 
w	(REQ8.2) Once a certain language is chosen, all menus must be displayed using the chosen language. 

