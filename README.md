# GOREMOVALS

![Tech Stack](resources/img/tech-stack-diagram.svg)

## Frontend

### App
- Partner
- Driver
- Customer

### Web
- Administrator (Manager)
- Customer

## Roles
- Administrator (Manager)
- Customer
- Fleet Owner (Partner)
- Driver

## Pages

### Customer Role (Customer Portal) (App, Web)
1. **Login** (App)
2. **SignUp** (App)
3. **Stops** (App, Web)
   1. Map
   2. Destination (Multi GeoLocationPicker)
4. **Trip Options** (App, Web)
   1. Floors
   2. Helpers
   3. Shuttles
   4. Date
   5. Time
   6. Coupon Code
   7. Notes
   8. Cost Breakdown (App)
5. **Trip Confirmation** (App, Web)
   1. Accept
   2. Decline
6. **Management (Trip Details)** (App, Web)
   1. Timeline
   2. Driver Details
   3. Summary
   4. Odometer (To Do: Check implementation)
   5. Duration
   6. Route & Stops

### Administrator (Manager) Role (Web)
1. **Dashboard**
   1. Calendar
   2. Unassigned Trips
   3. Active Trips
   4. Completed Trips
2. **Trips**
   1. Filters
3. **Partners**
4. **Payout**
5. **Invoices**
6. **Customers**
7. **Settings**
8. **Rate**
9. **Coupon**

### Partner & Driver Role (App)
1. **Dashboard** (Partner & Driver)
   1. Total Trips (Partner & Driver)
   2. New Trips (Partner & Driver)
   3. Vehicle (Driver)
   4. Driver Ratings (Driver)
   5. Total Drivers (Partner)
   6. Total Vehicles (Partner)
   7. Earnings (Partner)
2. **Trip Details** (Partner & Driver)
   1. Calendar (Partner & Driver)
   2. [Insert details]

- **Drivers (CRUD)** (Partner)
- **Vehicles (CRUD)** (Partner)
- **Profile** (Partner & Driver)


## Resources
- Third-party payment system
- Google API
- Apple API

## Backend

### Entities
- User
- Role
- Trip
  - Customer
  - Driver
  - Payout
  - Total Amount
- Trip Options
  - Floor (Type of flooring for the trip)
  - Shuttles (Shuttle services available)
  - Helpers (Additional help required)
  - Date
  - Time
  - Coupon Code
  - Notes
  - Destination
  - Status
  - Timeline
  - Odometer Open
  - Odometer Close
  - Duration Start
  - Duration End
- Fleet
  - Collection (Vehicle)
- Partner: User
  - Fleet
  - Bank Verification
  - Total Drivers
  - Total Vehicles
  - Bank Verification
  - Bank Account
- Bank Account
- Driver: User
  - Driver License
- Trip Status (Pending, Pay Now, Approved, View Invoice, Complete, In Progress)
- GeoLocation
- Vehicle
  - Vehicle Size (Truck Type)
  - License Plate (Registration Number)
  - License Expiry Date
  - Status
  - Model
  - Class
  - Body Type
  - Year
  - Joining Odometer
  - Rating
  - Documents/Images
- Vehicle Size (Truck Type)
- Coupons
- History (Timeline)
- Driver
  - Name
  - Contact Number
  - Vehicle Size (Truck Type)
- Payout
- Invoices
- Rate
- Coupon
- Document
- Notification

## Endpoints

### Customer Role (Customer Portal) (App, Web)
- **Login**: /login
- **SignUp**: /signup
- **Stops**: /stops
  - Map: /stops/map
  - Destination: /stops/destination
- **Trip Options**: /trip-options
  - Floors: /trip-options/floors
  - Helpers: /trip-options/helpers
  - Shuttles: /trip-options/shuttles
  - Date: /trip-options/date
  - Time: /trip-options/time
  - Coupon Code: /trip-options/coupon-code
  - Notes: /trip-options/notes
  - Cost Breakdown: /trip-options/cost-breakdown
- **Trip Confirmation**: /trip-confirmation
  - Accept: /trip-confirmation/accept
  - Decline: /trip-confirmation/decline
- **Management (Trip Details)**: /management
  - Timeline: /management/timeline
  - Driver Details: /management/driver-details
  - Summary: /management/summary
  - Odometer: /management/odometer
  - Duration: /management/duration
  - Route & Stops: /management/route-stops

### Administrator (Manager) Role (Web)
- **Dashboard**: /dashboard
  - Calendar: /dashboard/calendar
  - Unassigned Trips: /dashboard/unassigned-trips
  - Active Trips: /dashboard/active-trips
  - Completed Trips: /dashboard/completed-trips
- **Trips**: /trips
  - Filters: /trips/filters
- **Partners**: /partners
- **Payout**: /payout
- **Invoices**: /invoices
- **Customers**: /customers
- **Settings**: /settings
- **Rate**: /rate
- **Coupon**: /coupon

### Partner & Driver Role (App)
- **Dashboard** (Partner & Driver): /dashboard
  - Total Trips: /dashboard/total-trips
  - New Trips: /dashboard/new-trips
  - Vehicle: /dashboard/vehicle
  - Driver Ratings: /dashboard/driver-ratings
  - Total Drivers: /dashboard/total-drivers
  - Total Vehicles: /dashboard/total-vehicles
  - Earnings: /dashboard/earnings
- **Trip Details** (Partner & Driver): /trip-details
  - Calendar: /trip-details/calendar
  - [Insert details]: /trip-details/[insert-details]

- **Drivers (CRUD)** (Partner): /drivers
- **Vehicles (CRUD)** (Partner): /vehicles
- **Profile** (Partner & Driver): /profile


### Relationship
- In the future

### External Services
- Google API
- Apple API

## Questions
- What does each action on the Trips table mean?
- Is there any integration with bank accounts or payment systems?
- Partner Details -> Vehicle Details -> Status (Who is managing this status?)
- Questions about the odometer (When, who, and how is managing this value?)
- Can the Administrator role delete another administrator role user?

