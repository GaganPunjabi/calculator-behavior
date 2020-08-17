# Multiplication

## Scenarios

### Scenario: Multiplication of positive numbers
  
  Given Calculator is ON AND Screen is clear
  When I type in "positive number"
  And I press "Multiply"
  And I type in "positive number"
  And I press "equals"
  Then I see the "Multiplied number" as the result

### Scenario: Multiplication of positive number and a negative number
  
  Given Calculator is ON AND Screen is clear
  When I type in "positive number"
  And I press "Multiply"
  And I type in "negative number"
  And I press "equals"
  Then I see the "Multiplied negative number" as the result

### Scenario: Multiplication of more than two numbers

  Given Calculator is ON AND Screen is clear
  When I type in "number"
  And I press "multiply"
  And I type in "number"
  And I press "multiply"
  And I type in "number"
  Then I see the "left to right multiplied number" as result

### Scenario: Multiplication of negative numbers

  Given Calculator is ON AND Screen is clear
  When I type in "negative number"
  And I press "Multiply"
  And I type in "negative number"
  And I press "equals"
  Then I see the "Multiplied positive number" as the result

### Scenario: Zero value multiplication

  Given Calculator is ON AND Screen is clear
  When I type in "0"
  And I press "multiply"
  And I type in "number"
  And I press "equals"
  Then I see the "0" as the result

### Scenario: Identify operation

  Given Calculator is ON AND Screen is clear
  When I type in "number"
  And I press "multiply"
  And I type in 1
  And I press "equals"
  Then I see the "number" as the result

### Scenario: Decimal value multiplication
  
  Given Calculator is ON AND Screen is clear
  When I type in "decimal number"
  And I press "Multiply"
  And I type in "decimal number"
  And I press "equals"
  Then I see the "Multiplied number at most 2 decimal place" as the result

### Scenario: Fractional multiplication

  Given Calculator is ON AND Screen is clear
  When I type in "Fraction number"
  And I press "multiply"
  And I type in "Fraction number"
  And I press "equals"
  Then I see the "Multiplied number" as the result

### Scenario: Large number multiplication

  Given Calculator is ON AND Screen is clear
  When I type in "number"
  And I press "multiply"
  And I type in "number"
  And I press "equals"
  Then I see the result in e raise to the power
  
### Scenario: Pressing "multiply button" more than one time

  Given Calculator is ON AND Screen is clear
  And I type in "number"
  And I press "multiply"
  And I press "multiply"
  And I type in "number"
  And I press "equal"
  Then I see "Multiplied number" as the result

### Scenario: Interleaving operators

  Given Calculator is ON AND Screen is clear
  And I type in "number"
  And I press "plus"
  And I type in "number"
  And I press "multiply"
  And I type in "number"
  And I press "equal"
  Then I see "Compute from left to right" as the result

### Scenario: Decimal value capping

  Given Calculator is ON AND Screen is clear
  And I type in "decimal number"
  And I press "multiply"
  And I type in "number"
  And I press "equal"
  Then I see "Multiplied number with two digit precision"
  as the result
