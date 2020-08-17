# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given the visitor software can make graphs and store per day counts
  
  When the week ends
  
  Then a graph with visitors count per day is included in the report

Scenario: Alert when seating capacity is full

  Given the software knows how many seats are present
  
  When only 15% of the seats are empty
  
  Then the software issues an alert to facilities manager
