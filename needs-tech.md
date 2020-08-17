# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

 Given that I can store count value locally before switching off the server
 
 When The server fails or restarts
 
 Then server takes latest value from the local machine

Scenario: Reconcile counts if the sensor is offline for a while

 Given that the the sensor has a register
 
 When the sensor is offline
 
 Then the sensor stores the value until it is online
