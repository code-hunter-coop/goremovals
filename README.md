# GOREMOVALS

![Tech Stack](tech-stack-diagram.svg)

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
    1. Filters
4. **Payout**
    1. Filters
5. **Invoices**
     1. Filters
6. **Customers**
     1. Filters
     2. Actions
7. **Settings**
     1. Filters
     2. Actions
8. **Rate**
     1. Filters
     2. Actions
9. **Coupon**
     1. Filters
     2. Actions

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
   2. List
3. **Drivers (CRUD)** (Partner)
    1. List
    2. Actions
4. **Vehicles (CRUD)** (Partner)
    1. List
    2. Actions
5. **Profile** (Partner & Driver)
    1. List
    2. Actions

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

1. **Customer Role (Customer Portal) (App, Web)**
   - **Login**: /login
   - **SignUp**: /signup
   - **Stops**: /stops
     1. Map: /stops/map
     2. Destination: /stops/destination
   - **Trip Options**: /trip-options
     1. Floors: /trip-options/floors
     2. Helpers: /trip-options/helpers
     3. Shuttles: /trip-options/shuttles
     4. Date: /trip-options/date
     5. Time: /trip-options/time
     6. Coupon Code: /trip-options/coupon-code
     7. Notes: /trip-options/notes
     8. Cost Breakdown: /trip-options/cost-breakdown
   - **Trip Confirmation**: /trip-confirmation
     1. Accept: /trip-confirmation/accept
     2. Decline: /trip-confirmation/decline
   - **Management (Trip Details)**: /management
     1. Timeline: /management/timeline
     2. Driver Details: /management/driver-details
     3. Summary: /management/summary
     4. Odometer: /management/odometer
     5. Duration: /management/duration
     6. Route & Stops: /management/route-stops

2. **Administrator (Manager) Role (Web)**
   - **Dashboard**: /dashboard
     1. Calendar: /dashboard/calendar
     2. Unassigned Trips: /dashboard/unassigned-trips
     3. Active Trips: /dashboard/active-trips
     4. Completed Trips: /dashboard/completed-trips
   - **Trips**: /trips
     - Filters: /trips/filters
   - **Partners**: /partners
   - **Payout**: /payout
   - **Invoices**: /invoices
   - **Customers**: /customers
   - **Settings**: /settings
   - **Rate**: /rate
   - **Coupon**: /coupon

3. **Partner & Driver Role (App)**
   - **Dashboard** (Partner & Driver): /dashboard
     1. Total Trips: /dashboard/total-trips
     2. New Trips: /dashboard/new-trips
     3. Vehicle: /dashboard/vehicle
     4. Driver Ratings: /dashboard/driver-ratings
     5. Total Drivers: /dashboard/total-drivers
     6. Total Vehicles: /dashboard/total-vehicles
     7. Earnings: /dashboard/earnings
   - **Trip Details** (Partner & Driver): /trip-details
     1. Calendar: /trip-details/calendar


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
