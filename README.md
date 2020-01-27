# BankZecure Web Application

All the instructions are in the quest!

The fake customer accounts' credentials are listed [here](https://github.com/WildCodeSchool/quest-springboot-sql-injection/blob/master/FakeAccountsCredentials.md).

# Optional task: find out how to exploit the vulnerability in the SQL profile update:

Since I can inject some SQL-code in the input fields, my idea is to change the login credentials of someone other's account. 
So I can login with that changed credentials afterwards.
The following text entered in the password field changes the Identifier of Mr. Swift to '123456' and the Password to 'mypassword':

* mypassword', identifier = '123456' WHERE last_name = 'Swift' -- ;

Or - if you enter following text - all e-mail-addresses and passwords in the database will be set to the same
(e-mail-address like in the input field, password = "mypassword":
* mypassword' -- ;

Note: the "*" is not part of the injection code, it's md-formatting