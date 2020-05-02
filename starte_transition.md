# State Transition Test Case Design Technique

State Transition Test case design technique is one of the Black Box test design techniques.

Using state transition testing, we pick test cases from an application where we need to test different system transitions.  

We can apply this when an application gives a different output for the same input, depending on what has happened in the earlier state.

## Tools to represent state transitions

There are two main ways to represent or design state transition:

* state transition diagram  
* state transition table

## state transition diagram





## state transition table (STT)

There are different ways to create state transition tables.


### Example 1

The different states for a car:  

* stopped
* accelerating
* constant speed
* braking

|states|inputs|next state|
|---|---|---|
|stopped|press gas pedal more|accelerating|
|accelerating|keep gas pedal constant|constant speed|
|accelerating|switch to breke pedal|braking|
|constant speed|press gas pedal more|accelerating|
|constant speed|switch to brake pedal|braking|
|braking|switch to gas pedal; press gas pedal more|accelerating|
|braking|switch to gas pedal|constant speed|
|braking|keep braking|stopped|
|stopped||constant speed|
|stopped||braking|
||||
||||

