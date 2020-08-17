# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given the software can classify each person as patient, staff, specialist or patient visitor
  
  When the software submits a report
  
  Then it includes a graph with the average patients on working days and holidays

Scenario: Compute parking slots to reserve for visiting specialists

  Given the schedule and count of specialists visiting the hospital
  
  When the day begins
  
  Then the software indicates number of parking spots to be saved
