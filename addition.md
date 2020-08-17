# Addition
## Scenarios
### Scenario: Addition of two positive number
  
  Given Calculator is ON AND Screen is clear

  When I type in "positive number"
    And I press "plus"
    And I type in "positive number"
    And I press "equals"

  Then I see the "added number" as the result

### Scenario: Addition of a positive number and a negative number
  
  Given Calculator is ON AND Screen is clear

  When I type in "positive number"
    And I press "plus"
    And I type in "negative number"
    And I press "equals"
  
  Then I see the "added number" as the result
  
### Scenario: Addition of multiple positive numbers
  
  Given Calculator is ON AND Screen is clear

  When I type in "positive number"
    And I press "plus"
    And I type in "positive number"
    And I press "plus"
    AND I type in "positive number"
    And I press "plus"
    And I type in "positive number"
    And I press "equals"
    
  Then I see the "added number" as the result

### Scenario: Invalid combination of the sum is given
  
  Given Calculator is ON AND Screen is clear
   
  When I type in "positive number"
    And I press "plus"
    And I press "plus"
    And I press "equals"
  Then I see the "added number" as the result
  
### Scenario: Addition of fractions

  Given Calculator is ON AND Screen is clear
  When I type in "positive fraction number"
  And I press "plus"
  And I type in "positive fraction number"
  And I press "equals"
  Then I see the "added number" as the result

### Scenario: Addition of decimals
  
  Given Calculator is ON AND Screen is clear
  When I type in "positive decimal number"
  And I press "plus"
  And I type in "positive decimal number"
  And I press "equals"
  Then I see the "added number" as the result

### Scenario: Identify operation

  Given Calculator is ON AND Screen is clear
  When I type in 0
  And I press "plus"
  And I type in "number"
  And I press "equals"
  Then I see the "added number" as the result
  
### Scenario: Converse operation

  Given Calculator is ON AND Screen is clear
  And I type in "number one"
  And I press "plus"
  And I type in "number two"
  And I press "equals"
  Then I see the "number two + number one" as the result

### Scenario: Adding numbers where the result goes out of range

  Given Calculator is ON AND Screen is clear
  When I type in "number"
  And I press "plus"
  And I type in "number"
  And I press "equals"
  Then I see the error message stating out of the range message
