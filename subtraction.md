# Subtraction

## Scenarios

### Scenario: Subtraction of two positive numbers

Given Calculator is ON AND Screen is clear
When I type in "positive number"
And I press "minus"
And I type in "positive number"
And I press "equals"
Then I see the "subtracted number" as the result

### Scenario: Subtraction of positive and negative number
  
  Given Calculator is ON AND Screen is clear
  When I type in "positive number"
  And I press "minus"
  And I type in "negative number"
  And I press "equals"
  Then I see the "subtracted number" as the result

### Scenario: Subtraction of two negative numbers
  
  Given Calculator is ON AND Screen is clear
  When I type in "negative number"
  And I press "minus"
  And I type in "negative number"
  And I press "equals"
  Then I see the "subtracted number" as the result

### Scenario: Subtraction of fractions

  Given Calculator is ON AND Screen is clear
  When I type in "fraction number"
  And I press "minus"
  And I type in "fraction number"
  And I press "equals"
  Then I see the "subtracted number" as the result

### Scenario: Subtraction of decimals
  
  Given Calculator is ON AND Screen is clear
  When I type in "positive decimal number"
  And I press "minus"
  And I type in "positive decimal number"
  And I press "equals"
  Then I see the "subtracted decimal number" as the result

### Scenario: Subtraction of more than two numbers

  Given Calculator is ON AND Screen is clear
  When I type in "number"
  And I press "minus"
  And I type in "number"
  And I press "minus"
  And I type in "number"
  And I press "equals"
  Then I see the "subtracted number" as the result from left to right

### Scenario: Subtracting numbers where the result goes out of range

  Given Calculator is ON AND Screen is clear
  When I type in "maximum acceptable negative number"
  And I press "minus"
  And I type in " positive number"
  And I press "equals"
  Then I see the result within the range

### Scenario: Invalid input provided as input

  Given Calculator is ON AND Screen is clear
  When I type in "number"
  And I press "minus"
  And I press "minus"
  And I press "minus"
  Then I see the "subtracted number" as the result

### Scenario: Identify operation

  Given Calculator is ON AND Screen is clear
  When I type in "number"
  And I press "minus"
  And I type in 0
  And I press "equals"
  Then I see the "number" as the result

### Scenario: Converse operation

  Given Calculator is ON AND Screen is clear
  And I type in "operand two"
  And I press "minus"
  And I type in "operand one"
  Then I see the "subtracted number" not equal to
  operand two minus operand one as the result
