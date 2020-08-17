# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given the visitor software can make graphs and store per day counts
  
  When the week ends
  
  Then the software includes a graph with visitors count per day in the report

Scenario: Alert when seating capacity is full

  Given the software knows the number of seats are present
  
  When 15% of the seats are empty
  
  Then the software issues an alert to facilities manager
