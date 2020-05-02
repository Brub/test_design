# Decision Table Test Case Design Technique

Decision Table Test case design technique is one of the Black Box test design techniques.

This test technique is appropriate for functionalities which has logical relationships between inputs (if-else logic).  
In Decision table technique, we deal with combinations of inputs.  
To identify the test cases with decision table, we consider **conditions** and **actions**.  
We take **conditions** as inputs and **actions** as outputs.

## Example 1

login page validation. Allow user to login only when both the ‘User ID’ and ‘Password’ are entered correct.

Here the **Conditions** to allow user to login are Enter **Valid User Name** and Enter **Valid Password**.

The **Actions** performed are Displaying **home page** and Displaying an **error message that User ID or Password is wrong**.


| ID | Conditions/Actions | test case 1 | test case 2 | test case 3 | test case 4 |
|----|--------------------|-------------|------------|-------------|------------|
| condition 1| valid user id | T | T | F | F |
| condition 2| valid password | T | F | T | F |
| action 1| home page | execute | | | |
| action 2| show error message 'Invalid user credentials' | | execute  | execute  | execute |


**T** = true / **F** = false / **X** = not possible 

From the case 2 and case 3, we could identify that if one of the condition failed then the system will display an error message as Invalid User Credentials.

So I am eliminating one of the test case from case 2 and case 3 and concluding with the below tabular column.

| ID | Conditions/Actions | test case 1 | test case 2 | test case 3 |
|----|--------------------|-------------|------------|-------------|
| condition 1| valid user id | T | T | F |
| condition 2| valid password | T | F | F |
| action 1| home page | execute | | |
| action 2| show error message 'Invalid user credentials' | | execute  | execute  |