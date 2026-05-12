# Delivery Analyzer
This software was made to simulate a list of deliveries. It receives the user's input and then calculates the price of each delivery (also calculating its total value).
## How to use it?
- Node.js: To run this in your terminal, uncomment the first line by removing the // .
- Online Compilers: Copy and paste the code into your preferred online compiler
## Business Rules

This system calculates the daily closing payout for couriers based on logistical, weather, and productivity variables.

### Individual Calculation (Per Delivery)
- **Base Fee:** Every delivery starts with a flat rate of R$ 5.00.
- **Distance Fee:** The cost per kilometer depends on the vehicle used:
  - **Bicycle:** R$ 1.20 per km.
  - **Scooter:** R$ 1.80 per km.
- **Weight Surcharge:** Packages up to 5 kg have no extra fee. For every kilogram above 5 kg, an extra R$ 2.50 is added.
- **Weather Fee:** Deliveries made in the rain receive a flat hazard bonus of R$ 3.00.
- **Terrain Difficulty:** Deliveries passing through the "Historic Center" receive a 10% surcharge on top of that specific delivery's total value (calculated after summing all previous fees).

### Productivity Bonus
After all deliveries are inserted, the system evaluates the courier's overall performance. An extra bonus of R$ 25.00 is added to the final payout if the courier meets at least one of the following goals:
- More than 8 deliveries in the shift.
- Total distance of more than 40 km.