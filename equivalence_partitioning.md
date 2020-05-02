# Equivalence Partitioning

Equivalence Partitioning Test case design technique is one of the Black Box test design techniques.

Equivalence Partitioning is also known as Equivalence Class Partitioning.

In equivalence partitioning, inputs to the software or system are divided into groups that are expected to exhibit similar behavior, so they are likely to be proposed in the same way.

Each and every condition of particular partition (group) works as same as other.    
If a condition in a partition is valid, other conditions are valid too.  
If a condition in a partition is invalid, other conditions are invalid too.

It helps to reduce the total number of test cases from infinite to finite.   
The selected test cases from these groups ensure coverage of all possible scenarios.

Equivalence partitioning is applicable at all levels of testing.

## Example 1
Assume, we have to test a field which accepts Age 18 – 56

**Valid Input**: 18 – 56  
**Invalid Input**: less than or equal to 17 (<=17), greater than or equal to 57 (>=57)  

**Valid Class**: 18 – 56 = Pick any one input test data from 18 – 56  
**Invalid Class 1**: <=17 = Pick any one input test data less than or equal to 17  
**Invalid Class 2**: >=57 = Pick any one input test data greater than or equal to 57

We have one valid and two invalid conditions here.

## Example 2
Assume, we have to test a filed which accepts a Mobile Number of ten digits.  

**Valid input**: 10 digits  
**Invalid Input**: 9 digits, 11 digits

**Valid Class**: Enter 10 digit mobile number = 9876543210  
**Invalid Class**: Enter mobile number which has less than 10 digits = 987654321  
**Invalid Class**: Enter mobile number which has more than 11 digits = 98765432109

We have one valid and two invalid conditions here.