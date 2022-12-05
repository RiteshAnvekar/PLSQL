
OTP Generation and Validation:
The project aims to create a PLSQL code to generate and validate OTP linked to a mobile number.


Project:
We have 5 sections in the code:

1.	Table: It has the code to create a table with 4 columns which are Mobile number, OTP, Valid from time, and Valid to time.

2.	OTP Generation Procedure:  It has a code that is used to generate a 6-digit random number which is considered OTP and it is mapped against a mobile number. Once an OTP is generated it gets inserted into the table against the mobile number and the current date and time are logged in the column Valid from time. For the Valid to time column, we add 60 mins in the current date time and insert the resulting value in that column.

3.	Execution block for OTP Generation: This block of code is used to execute the OTP generation procedure.

4.	OTP Validation Procedure: In this block, we validate the mobile number and the generated OTP that is passed by the execution block and verify if the Mobile number and OTP are mapped against each other along with that we validate if the current system time lies between Valid from and Valid to time in the table. According to the validation result, a message is sent out to the execution block.

5.	Execution Block for Validating OTP: This block is used to execute the OTP Validation procedure where in we pass the mobile number and the generate OTP for validation.
