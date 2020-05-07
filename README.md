# CIS245-Python-Assignment9.1
Repository for assignment 9.1
# changes to include assignment 8 for repository.


#This program represents the functions of a Bank Account
print("hello bithub");

print("Hello bitHub");

class Bankaccount:
    """Attempt to represent a Bank Account."""
    def__init__(self,accountnumber,balance,interestrate,fees,minimumbalance)
    self.accountnumber = accountnumber
    self.balance = 0
    self.interestrate = 0.02
    self.fees = 5
    self.minimumbalance = 50
    
    #represents a withdrawl
    def withdrawl(self):
        amount = float(input("Amount you want to withdraw"))
        self.balance -= amount
        print("\n Amount withdrawn: ", amount)
        print("\n New Balance: ", balance)
    
    #represents a deposit
    def deposit(self):
        amount = float(input("Amount you want to deposit "))
        self.balance += amount
        print("\n Amount deposited ", amount)
        print("\n New Balance: ", balance)
    
    #represents check balance
    def get_balance(self):
        new_balance = balance - withdrawl + deposit
        return int(new_balance)


print("Anytime you want to exit: input exit in input")

#sub class for checking
class checkingaccount(Bankaccount):
    """Represents the Bank account, specifically checking."""
    def__init__(self,fees,minimumbalance)
    """Initialize attributes of the parent class.
        Then specific attributes to checking account. """
    super().__init__(fees, minimumbalance)

    def deductfees(self):
        new_balance = balance - fees
        print("Charged overdraft fee: ", new_balance)

    def checkminimumbalance(self):
        try:
            balance >= 50
        except balance < 50:
            print("Your account is below minimum balance")
        else:
            print(balance)

#sub class for savings
class Savingsaccount(Bankaccount):
    """Represents the bank account, specifically savings"""
    def__init__(self, interestrate)
    """Initialize attributes of the parent class.
        Then specific attributes to savings account. """
    super().__init__(interestrate)

    def addinterest(self):
        self.new_balance = int(balance * 1.02)
        print("Balance with interest ", new_balance)

#user input to exit
user_input = input()
if user_input == 'exit':
    sys.exit()

