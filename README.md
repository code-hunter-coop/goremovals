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

### Customer Portal (App, Web, Mobile Web)
1. **Login** (App, Web)
2. **SignUp** (App, Web)
3. **Forgot Password** (App, Web)
4. **Stops** (App, Web)
   1. Map with polylines
   2. List of Stops Multi GeoLocationPicker (Pick-Up,  Drop-off) 
   3. Vehicle type (PopUp window)
5. **Trip Options** (App, Web)
   1. Floors
   2. Helpers
   3. Shuttles
   4. Date
   5. Time
   6. Coupon Code
   7. Notes
6. **Cost Breakdown** (App, Web)
   1. Basefare 
   2. Cost per KM
   3. Options
   4.  Cupon
   5.  Total
   6.  Accept (redirection to Login or SignUp page)
   7.  Decline (PopUp window with reasons)
7.  **Confirmation** (App, Web)
   1. List of Stops
   2. Options
   3. Date
   4. Cost
   5. Accept (Booking has been confirmed)
   6. Decline
8.  **Bookings Management** (App, Web)
    1. List Bookings with filters
       1. Id
       2. Time (start time)
       3. Vehicle (max weight)
       4. Origin (start place pick-up point)
       5. Destination (drop-off points)
       6. Status (Pending, Approved, Completed, inProgres, View invoice, PayNow)
       7. Pay Now (what service is used? )

9. **Trip Details**
    1. Timeline (history of trip statuses)
    2. Driver Details
    3.  Summary (Booking options)
    4.  Odometer (To Do: Check implementation)
    5.  Duration
    6.  Route & Stops
10. **Make Payment**
    1.  Unknown

### Admin Portal (Web)
1. **Dashboard**
   1. Calendar
   2. Calendar list of trips
   3. Unassigned Trips
   4. Active Trips
   5. Completed Trips
   6. TripDetails (PopUp window)
   7. Actions
      1. AssignDriver
      2. Update stops statuses (not all statuses)
2. **Trips**
   1. Filters
   2. List Bookings with filters
       1. Id
       2. Driver
       3. Time (start time)
       4. Rate
       5. Helpers
       6. Flour
       7. Cupon
       8. Payout
       9. TotalAmount
       10. Action
   3. Actions
      1. AssignDriver
      2. Update stops statuses (not all statuses)
   4. TripDetails (PopUp window)
3. **Partners**
    1. Filters
    2. List of Partners
       1. JointDate
       2. FleetId
       3. FleetOwner
       4. Phone
       5. Email
       6. Status (active, not active)
       7. TotalTrips
       8. TotalDrivers
       9. TotalVehciles
       10. BankVarification
       11. Action
5. **PartnerDetails**
   1. Name
   2. email
   3. phone
   4. Address
   5. BankAccount
   6. BankAccount valid
   7. Documents
6. **DriverDetalis**
   1. Name
   2. email
   3. phone
   4. Address
   5. Status (active)
   6. DateOfBirth
   7. ShowTransactons
   8. BlockDriver
   9. OperatingProvinces
7. **VehicleDetails**
   1. Id
   2. Staus (Waiting)
   3. Driver
   4. Model
   5. VehicleMake Brend (Hundai)
   6. VehicleClass (1,3 TonTrack)
   7. VehicleBodyType 
   8. Year
   9. JoiningOdometer
   10. Registration Number
   11. LicenseExpireDate
   12. Documents
8. **Payout**
    1. Filters
    2. List
       1. Id
       2. Partner
       3. Status (Active)
       4. Payout (Payout)
       5. TotalTrips
       6. StartDate
       7. EndDate
       8. DueDate
       9. Dedications
       10. TotalAmount
9. **PayoutDetalis**
   1.  ParthnerContacts
   2.  ListRemovalTrips
10. **Make Payment**
    1.  Unknown
11. **Invoices**
     1. Filters
      2.  List
          1.  Id
          2.  Removal Id
          3.  Status ( Paid)
          4.  Rates (???)
          5.  InvoceDate
          6.  Cupon
          7.  Discount
          8.  Amount
          9.  ViewInvoce
          10. Action
12. **InvoiceDetails**
    1.  Unknown Format
13. **Customers**
     1. Filters
     2. List
        1. Id
        2. AddedDateTime
        3. Name
        4. Status (Active, Inactive)
        5. Email
        6. Phone
        7. Type (Business)
     3. Actions
14. **Settings**
     1. Filters
     2. List of admin users
        1. Id
        2. email
        3. organization
        4. Role
        5. Action
     3. Actions
15. **UserDetalis**
    1.  FirstName
    2.  LastName
    3.  Role
    4.  Email
    5.  OldPassword
    6.  NewPassword
16. **Rate**
     1. Filters
     2. List of rates
        1. Id
        2. Name
        3. Status
        4. Basefare
        5. Cost per km
        6. TimeTrashold
        7. Cost per hr
        8. Cost per helper
        9. Cost per floor
        10. Action
     3. Actions
17. **RateCreateEdit**
    1.  Name
    2.  Status
    3.  Basefare
    4.  Cost per km
    5.  TimeTrashold
    6.  Cost per hr
    7.  Cost per helper
    8.  Cost per floor
18. **Company**
    1.  Name
    2.  Address
    3.  City
    4.  State
    5.  ZipCode
    6.  State
    7.  Phone
    8.  VatNumber
    9.  Document
19. **Coupon**
     1. Filters
        1. List of coupons
           1. Id
           2. Name
           3. Status
           4. Code
           5. Discount
     2. Actions
20. **CuponCreateEdit**
    1. Name
     2. Status
     3. Code
     4. Discount

### Partner & Driver Role (App)
1. **Dashboard** (Partner & Driver)
   1. Total Trips (Partner & Driver)
   2. New Trips (Partner & Driver)
   3. Total Drivers (Partner)
   4. Total Vehicles (Partner)
   5. Vehicle (Driver)
   6. Driver Ratings (Driver)
   7. Earnings (Partner)
2. **Trip Details** (Partner & Driver)
   1. Map
   2. Overview
      1. Id
      2. CustomerName
      3. CustomerPhone
      4. DateTime
      5. Helpers
      6. Notes
      7. PaymentStatus (Unpaid)
      8. Discount
      9. Discount Total Excel
      10. Floors
   3.  RemovalDetalis
          1.  VahicleType
          2.  RemovalType Flat
          3.  ElevatorStatus (True)
          4.  Categories: Appilances, Boxes, Beding, Chairs + Tables
          5.  Description: L-Shape Couch Ottoman, Coffe Table, Dining Room Table + 6 Chairs
   4. Related Driver
      1. Id
      2. Phone
      3. Photo
       
   5. TimeLine (Partner & Driver)
   6. List
3. **Calendar View** (Partner & Driver)
   1. Calendar
   2. List of current and future events
4. **Drivers** (Partner)
    1. List
    2. Actions
5. **Driver Detaild Add Edit** (Partner) **Edit** (Driver)
   1. Name
   2. Email
   3. Status
   4. Date of Birth
   5. Show Transactions
   6. Block Driver
   7. Address
   8. Documents
6. **Vehicles** (Partner)
    1. List
    2. Actions
7. **Vehicle Details Add Edit** (Partner) **View** (Driver)
   1. Id
   2. Status (Waiting)
   3. Driver
   4. Model
   5. Brand
   6. Class
   7. Body Type
   8. Year
   9. Joining Odometer
   10. Registration Number
   11. License Expiry Date
   12. Documents
8.  **Earnings** (Partner)
    1.  Earning for the Period
    2.  Next Payout
    3.  List of Earnigs by Driver
9. **Earning Details** (Partner)
   1.  Total Removals
       1.  Total Distance (km)
       2.  Total Duration (Hr)
       3.  Dedication Amount
       4.  Dedication Reasoning
       5.  Gross Total Payout
       6.  Net Total Payout
   2. List of Removal Trips
      1. Filters
10. **Profile** (Partner & Driver)
    1. List
    2. Actions
 11. **Notification**  (Partner & Driver)

## Resources
- Third-party payment system
- Google API
- Apple API

## Backend

### Entities
- User
- Role
- Organisation
- Stop
    - GeoLocation
    - Pick-up
    - Drop-off
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
- TripStatus
  - BookingMode
  - BookingApproved
  - DriverHeadingToPickUp
  - DriverAtPociUpLocation
  - PackingComplete
  - DriverHeadingToNextStop
  - TripCompleted
  - InvoiceSubmited
  - PaymentReceived
- Fleet
  - Collection (Vehicle)
- Partner: User
  - Full name
  - email
  - phone
  - address
  - Joining
  - Fleet
  - Bank Verification
  - Total Drivers
  - Total Vehicles
  - Bank Verification
  - Bank Account
- Bank Account
- Driver: User
  - Driver License
  - email
  - phone
  - Address
  - DateOfBirth
  - ShowTransacions
  - Blocked (true, false)
  - DriverStatus
  - OperatingProvinces
  - Documents (images)
- DriverStauts (Verified)
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
  - Vehicle MaxWeight (ToDo check this parameter)
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
     3. Pop
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
**Customer**
- Page "List of stops". Does the customer choose the difference between pick-up and drop-off or does it all have the same meaning for the trip? Are the stop sequences calculated by the business logic or just how the customer chooses?
- Page "Cost breakdown". What is the logic under all calculations?
- Page "Booking management". Time - is it start trip time? Origin - is it the start location? Vaehicle - is this maxWeight or vaehicle type? This parameter is absent on the Vehicles page. Where are this parameter located?
**Admin Portal**
- Page "Dashboard" -> Edit Removal Trips -> Change stops statuses. What about other states? Who and when changing them?
- Page Partners -> Partner Details -> Driver -> block (blocked, unblocked). What does this action do? Does this make the driver inactive for the partner to choose in the future or something else? 
- Page Partners -> Partner Details -> ShowTransactions - Hide. What does this mean?
- Page Payouts -> ActivePayouts -> Dedications. What does this mean?
- Page Invices -> Action View Invoice. Is there an example of the invoice?
- Page Settings -> Users -> List column "Organisation". Is this a company? How many Organisations are there? Who and were managing them?
- Page Settings ->Settings -> UserDetails -> Action "Set Password". If these options are for each user in the list how can you know the old password? Usually just set a new password.
- Page Settings ->Settings -> CompanyDetails -> two times field State. Is it better to change one of them to country? 



- Is there any integration with bank accounts or payment systems?
- Partner Details -> Vehicle Details -> Status (Who is managing this status?)
- Questions about the odometer (When, who, and how is managing this value?)
- Can the Administrator role delete another administrator role user?