![Tech Stack](resources/img/tech-stack-diagram.svg)

# Tech Stack
- Business logic and REST API can be built using C# program language and modern cross-platform framework .Net. It has libraries to work with all types of databases and file structures so depending on the chosen production platform can be used by specific databases and file provider (PostgreSQL, MSSQl, MySql, CosmDb etc.).
- Web and MobileWeb can be built also using C# program language and cross-platform .Net Blazor framework. All C# code can be located on-premises or on the cloud (the most popular platforms on the market are Azure and AWS).

# Frontend

### App
- Partner
- Driver
- Customer

### Web
- Administrator (Manager)
- Customer

### Mobile Web
- Customer

## Roles
- Administrator (Manager)
- Customer
- Fleet Owner (Partner)
- Driver


## Pages

### Customer Portal (App, Web, Mobile Web)
1. **Login**
2. **Sign Up**
3. **Forgot Password**
4. **Stops**
   - Map with polylines
   - List of Stops Multi GeoLocationPicker (Pick-Up, Drop-off)
   - Vehicle type (PopUp window)
5. **Trip Options**
   - Floors
   - Helpers
   - Shuttles
   - Date
   - Time
   - Coupon Code
   - Notes
6. **Cost Breakdown**
   - Base Fare
   - Cost per KM
   - Options
   - Coupon
   - Total
   - Accept (redirection to Login or Sign Up page)
   - Decline (PopUp window with reasons)
7. **Confirmation**
   - List of Stops
   - Options
   - Date
   - Cost
   - Accept (Booking has been confirmed)
   - Decline
8. **Bookings Management**
   - List Bookings with filters
     - Id
     - Time (start time)
     - Vehicle (max weight)
     - Origin (start place pick-up point)
     - Destination (drop-off points)
     - Status (Pending, Approved, Completed, in Progress, View invoice, Pay Now)
     - Pay Now (what service is used?)

9. **Trip Details**
   - Timeline (history of trip statuses)
   - Driver Details
   - Summary (Booking options)
   - Odometer (To Do: Check implementation)
   - Duration
   - Route & Stops
10. **Make Payment**
    - Unknown

### Admin Portal (Web)
1. **Login**
2. **Sign Up**
3. **Forgot Password**
1. **Dashboard**
   - Calendar
   - Calendar list of trips
   - Unassigned Trips
   - Active Trips
   - Completed Trips
   - Trip Details (PopUp window)
   - Actions
     - Assign Driver
     - Update stops statuses (not all statuses)
2. **Trips**
   - Filters
   - List Bookings with filters
     - Id
     - Driver
     - Time (start time)
     - Rate
     - Helpers
     - Floor
     - Coupon
     - Payout
     - Total Amount
     - Action
   - Actions
     - Assign Driver
     - Update stops statuses (not all statuses)
   - Trip Details (PopUp window)
3. **Partners**
   - Filters
   - List of Partners
     - Join Date
     - Fleet Id
     - Fleet Owner
     - Phone
     - Email
     - Status (active, not active)
     - Total Trips
     - Total Drivers
     - Total Vehicles
     - Bank Verification
     - Action
4. **Partner Details**
   - Name
   - Email
   - Phone
   - Address
   - Bank Account
   - Bank Account valid
   - Documents
5. **Driver Details**
   - Name
   - Email
   - Phone
   - Address
   - Status (active)
   - Date of Birth
   - Show Transactions
   - Block Driver
   - Operating Provinces
6. **Vehicle Details**
   - Id
   - Status (Waiting)
   - Driver
   - Model
   - Vehicle Make Brend (Hyundai)
   - Vehicle Class (1,3 Ton Track)
   - Vehicle Body Type
   - Year
   - Joining Odometer
   - Registration Number
   - License Expire Date
   - Documents
7. **Payout**
   - Filters
   - List
     - Id
     - Partner
     - Status (Active)
     - Payout (Payout)
     - Total Trips
     - Start Date
     - End Date
     - Due Date
     - Deductions
     - Total Amount
8. **Payout Details**
   - Partner Contacts
   - List Removal Trips
9. **Make Payment**
   - Unknown
10. **Invoices**
    - Filters
    - List
      - Id
      - Removal Id
      - Status (Paid)
      - Rates (???)
      - Invoice Date
      - Coupon
      - Discount
      - Amount
      - View Invoice
      - Action
11. **Invoice Details**
    - Unknown Format
12. **Customers**
    - Filters
    - List
      - Id
      - Added Date Time
      - Name
      - Status (Active, Inactive)
      - Email
      - Phone
      - Type (Business)
    - Actions
13. **Settings**
    - Filters
    - List of admin users
      - Id
      - Email
      - Organization
      - Role
      - Action
    - Actions
14. **User Details**
    - First Name
    - Last Name
    - Role
    - Email
    - Old Password
    - New Password
15. **Rate**
    - Filters
    - List of rates
      - Id
      - Name
      - Status
      - Base Fare
      - Cost per km
      - Time Threshold
      - Cost per hr
      - Cost per helper
      - Cost per floor
      - Action
    - Actions
16. **Rate Create/Edit**
    - Name
    - Status
    - Base Fare
    - Cost per km
    - Time Threshold
    - Cost per hr
    - Cost per helper
    - Cost per floor
17. **Company**
    - Name
    - Address
    - City
    - State
    - Zip Code
    - Phone
    - Vat Number
    - Document
18. **Coupon**
    - Filters
    - List of coupons
      - Id
      - Name
      - Status
      - Code
      - Discount
    - Actions
19. **Coupon Create Edit**
    - Name
    - Status
    - Code
    - Discount

### Partner & Driver Role (App)
1. **Login**
2. **Sign Up**
3. **Forgot Password**
1. **Dashboard** (Partner & Driver)
   - Total Trips (Partner & Driver)
   - New Trips (Partner & Driver)
   - Total Drivers (Partner)
   - Total Vehicles (Partner)
   - Vehicle (Driver)
   - Driver Ratings (Driver)
   - Earnings (Partner)
2. **Trip Details** (Partner & Driver)
   - Map
   - Overview
     - Id
     - Customer Name
     - Customer Phone
     - Date Time
     - Helpers
     - Notes
     - Payment Status (Unpaid)
     - Discount
     - Discount Total Excel
     - Floors
   - Removal Details
     - Vehicle Type
     - Removal Type Flat
     - Elevator Status (True)
     - Categories: Appliances, Boxes, Bedding, Chairs + Tables
     - Description: L-Shape Couch Ottoman, Coffee Table, Dining Room Table + 6 Chairs
   - Related Driver
     - Id
     - Phone
     - Photo
   - Timeline (Partner & Driver)
   - List
3. **Calendar View** (Partner & Driver)
   - Calendar
   - List of current and future events
4. **Drivers** (Partner)
   - List
   - Actions
5. **Driver Details Create Edit** (Partner) **View Edit** (Driver)
   - Name
   - Email
   - Status
   - Date of Birth
   - Show Transactions
   - Block Driver
   - Address
   - Documents
6. **Vehicles** (Partner)
   - List
   - Actions
7. **Vehicle Details Create Edit** (Partner) **View** (Driver)
   - Id
   - Status (Waiting)
   - Driver
   - Model
   - Brand
   - Class
   - Body Type
   - Year
   - Joining Odometer
   - Registration Number
   - License Expiry Date
   - Documents
8. **Earnings** (Partner)
   - Earning for the Period
   - Next Payout
   - List of Earnings by Driver
9. **Earning Details** (Partner)
   - Total Removals
     - Total Distance (km)
     - Total Duration (Hr)
     - Dedication Amount
     - Dedication Reasoning
     - Gross Total Payout
     - Net Total Payout
   - List of Removal Trips
     - Filters
10. **Profile** (Partner & Driver)
    - List
    - Actions
11. **Notification**  (Partner & Driver)


### Resources
- Third-party payment system
- Google API
- Apple API

### Summary
- App pages (21)
- Web pages (29)
- Mobile Web pages (10)


# Backend

## Entities

### User
- Name
- Email
- Phone
- Address
- Date of Birth
- Show Transactions
- Blocked (true/false)
- Role
- Organization

### Role
- Name

### Organization
- Name
- Address
- City
- State
- ZipCode
- Phone
- VatNumber
- Document

### Stop
- Location
- Pick-up
- Drop-off

### Trip
- Customer
- Driver
- Payout
- Total Amount
- Status
- Timeline
- Odometer Open
- Odometer Close
- Duration Start
- Duration End

### Trip Options
- Floors
- Shuttles
- Helpers
- Date
- Time
- Coupon Code
- Notes
- Destination

### Fleet
- Vehicles

### Partner
- Full Name
- Email
- Phone
- Address
- Joining Date
- Fleet
- Bank Verification
- Total Drivers
- Total Vehicles
- Bank Account

### Driver
- Name
- Email
- Phone
- Address
- Date of Birth
- Show Transactions
- Blocked (true/false)
- Status
- Driver License
- Operating Provinces
- Documents

### Vehicle
- Vehicle Size (Truck Type)
- License Plate (Registration Number)
- License Expiry Date
- Status
- Model
- Brand
- Class
- Body Type
- Year
- Joining Odometer
- Rating
- Documents/Images
- Vehicle Max Weight

### Payout
- Partner
- Status
- Total Trips
- Start Date
- End Date
- Due Date
- Deductions
- Total Amount

### Invoice
- Removal Id
- Status
- Rates
- Invoice Date
- Coupon
- Discount
- Amount

### Rate
- Name
- Status
- Base Fare
- Cost per km
- Time Threshold
- Cost per hr
- Cost per helper
- Cost per floor

### Coupon
- Name
- Status
- Code
- Discount

### Document
- Type
- Content

### Notification
- Sender
- Receiver
- Message


## Endpoints

1. **Customer Role (Customer Portal)**
   1. **Login**: `/api/login`
   2. **SignUp**: `/api/signup`
   3. **Forgot Password**: `/api/forgot-password`
   4. **Stops**: `/api/stops`
      1. Map: `/api/stops/map`
      2. List of Stops Multi GeoLocationPicker (Pick-Up, Drop-off): `/api/stops/list`
      3. Vehicle type (PopUp window): `/api/stops/vehicle-type`
   5. **Trip Options**: `/api/trip-options`
      1. Floors: `/api/trip-options/floors`
      2. Helpers: `/api/trip-options/helpers`
      3. Shuttles: `/api/trip-options/shuttles`
      4. Date: `/api/trip-options/date`
      5. Time: `/api/trip-options/time`
      6. Coupon Code: `/api/trip-options/coupon-code`
      7. Notes: `/api/trip-options/notes`
   6. **Cost Breakdown**: `/api/cost-breakdown`
   7. **Confirmation**: `/api/confirmation`
   8. **Bookings Management**: `/api/bookings-management`
   9. **Trip Details**: `/api/trip-details`
   10. **Make Payment**: `/api/make-payment`

2. **Administrator Role (Web)**
   1. **Dashboard**: `/api/dashboard`
   2. **Trips**: `/api/trips`
   3. **Partners**: `/api/partners`
   4. **Payout**: `/api/payout`
   5. **Invoices**: `/api/invoices`
   6. **Customers**: `/api/customers`
   7. **Settings**: `/api/settings`
   8. **Rate**: `/api/rate`
   9. **Coupon**: `/api/coupon`

3. **Partner & Driver Role (App)**
   1. **Dashboard**: `/api/dashboard`
   2. **Trip Details**: `/api/trip-details`
   3. **Calendar View**: `/api/calendar-view`
   4. **Drivers (CRUD)**: `/api/drivers`
   5. **Driver Details Create/Edit**: `/api/driver-details`
   6. **Vehicles (CRUD)**: `/api/vehicles`
   7. **Vehicle Details Create/Edit**: `/api/vehicle-details`
   8. **Earnings**: `/api/earnings`
   9. **Earning Details**: `/api/earning-details`
   10. **Profile**: `/api/profile`
   11. **Notification**: `/api/notification`

### Summary
- EndPoints (30)

### Relationship
- In the future

### External Services
- Google API
- Apple API

## Suggestions
- The terms "Fleet Owner" and "Partner" are equally used in business logic and app views. May we use only the "Partner" term to simplify app logic? 
- The terms "Removal", "Trips", "Removal Trips" and "Bookings" are equally used in business logic and app views. May we use only one term to simplify app logic? Our suggestion is also to think about the common term "Order".
- The role "Administrator" has all the characteristics of the "Manager" role. Maybe it's better to use this role name.

## Questions
**Customer**
- Page "List of stops". Does the customer choose the difference between pick-up and drop-off or does it all have the same meaning for the trip? Are the stop sequences calculated by the business logic or only by customer choices?
- Page "Enter trip options" field "Shuttles". What does this mean?
- Page "Cost breakdown". Do the calculation options depend only on "Vehicle Type" from "Rate" data?
- Page "Booking management". Time - is it start trip time? Origin - is it the start location? Vehicle - is this Vehicle Type?
**Admin Portal**
- Page "Dashboard" -> Edit Removal Trips -> Change stops statuses. What about other states? Who and when changing them?
- Page Partners -> Partner Details -> Driver -> block (blocked, unblocked). What does this action do? Does this make the driver inactive for the partner to choose in the future or something else? 
- Page Partners -> Partner Details -> ShowTransactions - Hide. What does this mean?
- Page Payouts -> ActivePayouts -> Dedications. What does this mean?
- Page Invices -> Action View Invoice. Is there an example of the invoice?
- Page Settings -> Users -> List column "Organisation". Is this a company? How many Organisations are there? Who and were managing them?
- Page Settings ->Settings -> UserDetails -> Action "Set Password". If these options are for each user in the list how can you know the old password? Usually just set a new password.
- Page Settings ->Settings -> CompanyDetails -> two times field State. Is it better to change one of them to country? 

**Business Logic**
- By deleting objects ("Users", "Vehicles" etc.) do you want to permanently delete this data from all tables without the opportunity to check them in the future or do you want to change the status to "inactive" to have the opportunity to check this data in the future?
- Does the program need extra logik for refounding?
- Does the client can pay with different parts for one "Trip"? Are there different types of payment like "payment before the trip", "payment after the trip" etc.?
- Is there any mechanism or API for integration with bank accounts or payment systems?
- Questions about the odometer (When, who, and how is managing this value?)
- Time Trash Hold - who, when and how can use this parameter?
- Can a user with the administrator (manager) role delete another user with the administrator (manager) role?
