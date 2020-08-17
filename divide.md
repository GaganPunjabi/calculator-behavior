# Division

## Scenarios

### Scenario: Division of positive numbers

Given Calculator is ON AND Screen is clear
When I type in "number"
And I press "divide"
And I type in "number"
And I press "equals"
Then I see the "divided number" as the result

### Scenario: Division by zero

Given Calculator is ON AND Screen is clear
When I type in "number"
And I press "divide"
And I type in "zero"
And I press "equals"
Then I see the "cannot divide the number by zero" as the result

### Scenario: Divide zero by any number
  
  Given Calculator is ON AND Screen is clear
  When I type in "zero"
  And I press "divide"
  And I type in "number"
  And I press "equals"
  Then I see "zero" as the result

### Scenario: Divide positive number with a negative number

  Given Calculator is ON AND Screen is clear
  When I type in "operand one" positive
  And I press "divide"
  And I type in "operand two" negative
  And I press "equals"
  Then I see the "negative divided number" as the result

### Scenario: Divide the negative number with a negative number

  Given Calculator is ON AND Screen is clear
  When I type in "operand one" negative
  And I press "divide"
  And I type in "operand two" negative
  And I press "equals"
  Then I see the "positive number" as the result

### Scenario: Symmetric division
  
  Given Calculator is ON AND Screen is clear
  When I type in "number one"
  And I press "divide"
  And I type in "number two"
  And I press "equals"
  Then I see the "number" not equal number two divides
  number one to  as the result

### Scenario: Division when both operands are 0
  
  Given Calculator is ON AND Screen is clear
  When I type in "zero"
  And I press "divide"
  And I type in "zero"
  And I press "equals"
  Then I see the "undefined" as the result

### Scenario: Recurring decimal case

  Given Calculator is ON AND Screen is clear
  When I type in "number"
  And I press "divide"
  And I type in "number"
  And I press "equals"
  Then I see the "at most two precision" as the result

### Scenario: Divided operator pressed twice

  Given Calculator is ON AND Screen is clear
  When I type in "number"
  And I press "divide"
  And I Press "divide"
  And I type in "number"
  And I press "equals"
  Then I see "divided number" as the result

### Scenario: Division by fractions

  Given Calculator is ON AND Screen is clear
  When I type in "number"
  And I press "divide"
  And I type in "fraction number"
  Then I see "divided number" as the result

### Scenario: Division of more than 2 numbers

  Given Calculator is ON AND Screen is clear
  When I type in "number"
  And I press "divide"
  And I type in "number"
  And I press "divide"
  And I type in "number"
  And I press "equals"
  Then I see the "left to right division" as the result

### Scenario: Interleaving operators

  Given Calculator is ON AND Screen is clear
  And I type in "number"
  And I press "plus"
  And I type in "number"
  And I press "divide"
  And I type in "number"
  And I press "equal"
  Then I see "Compute from left to right" as the result
