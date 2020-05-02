# Boundary Value Analysis (BVA)

Equivalence Partitioning Test case design technique is one of the Black Box test design techniques.

Boundary value analysis is based on testing the boundary values of valid and invalid partitions.  

Every partition has its maximum and minimum values and these maximum and minimum values are the boundary values of a partition.

A boundary value for a valid partition is a **valid boundary value**.  
Similarly a boundary value for an invalid partition is an **invalid boundary value**.  

Tests can be designed to cover both valid and invalid boundary values.  
When designing test cases, a test for each boundary value is chosen.

For each boundary, we test +/-1 in the least significant digit of either side of the boundary.

Boundary value analysis can be applied at all test levels.

## Example 1

Assume, we have to test a field which accepts Age 18 – 56

Minimum valid boundary value is 18  
Maximum valid boundary value is 56

**Valid Inputs**: 18,19,55,56  
**Invalid Inputs**: 17 and 57

Test case 1: Enter the value 17 (=18-1) = Invalid

Test case 2: Enter the value 18 = Valid

Test case 3: Enter the value 19 (=18+1) = Valid

Test case 4: Enter the value 55 (=56-1) = Valid

Test case 5: Enter the value 56 = Valid

Test case 6: Enter the value 57 (=56+1) = Invalid

## Example 2

Assume we have to test a text field (Name) which accepts the length between 6-12 characters.

Minimum valid boundary value is 6  
Maximum valid boundary value is 12

**Valid text length**: is 6, 7, 11, 12
**Invalid text length**: is 5, 13

Test case 1: Text length of 5 (min-1) = Invalid

Test case 2: Text length of exactly 6 (min) = Valid

Test case 3: Text length of 7 (min+1) = Valid

Test case 4: Text length of 11 (max-1) = Valid

Test case 5: Text length of exactly 12 (max) = Valid

Test case 6: Text length of 13 (max+1) = Invalid











