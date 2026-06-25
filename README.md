# Mandir-Lifts
**Core Features:**

Two-panel input form (Kishores on left, Drivers on right, Mandir location at top)
Starts completely empty with no pre-filled data
UK postcode validation with inline error messages (accepts spaces or no spaces)
Add/remove kishores and drivers with one click
Auto-uppercase postcode inputs

Route Optimization:

Drivers automatically do multiple trips if kids exceed seat capacity
Intermediate trips return to Mandir, final trip goes to driver's home
Nearest-neighbor algorithm for quickest routes
Greedy VRP solver that minimizes total travel distance
Balances workload across drivers respecting seat limits

Results Display:

Driver cards showing name, home postcode, and all trips
Trip labels when driver does multiple trips
Stops listed with order, names, and postcodes
Seat utilization displayed (e.g., 3/4 seats used)
Total distance per trip in kilometers
Google Maps integration with pre-loaded waypoints and turn-by-turn nav
Unassigned kishores clearly marked with helpful message to add another driver

**This is the changes i made from first prototype to this:**
Input & Data Entry:

Added postcode validation for all inputs (accepts spaces or no spaces)
Added inline error messages for invalid postcodes

Route Logic:

Added multi-trip support (drivers do multiple trips if needed)
Changed intermediate trip destinations from driver's home to Mandir (return to pick up more kids)
Added nearest-neighbor routing for quickest routes
Optimized for minimizing total travel distance

Results Display:

Added trip labels (Trip 1, Trip 2, etc.) when driver does multiple trips
Added trip dividers separating multiple trips visually
Changed final destination label from "Home" to show "Mandir (Return)" for non-final trips
Updated unassigned section header from "Still need rides" to "Remainder"
Added helpful message to add another driver for unassigned kishores
