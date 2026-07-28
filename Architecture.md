                              CAB BOOKING MANAGEMENT SYSTEM
                                      (ServiceNow)

+--------------------------------------------------------------------------------+
|                                 Presentation Layer                             |
|--------------------------------------------------------------------------------|
|  Employee Portal     |     Driver Portal      |     Admin Workspace            |
|  - Login             |     - View Trips       |     - Manage Bookings          |
|  - Book Cab          |     - Update Status    |     - Assign Driver            |
|  - View Bookings     |                        |     - Manage Vehicles          |
+-----------------------------------+--------------------------------------------+
                                    |
                                    v
+--------------------------------------------------------------------------------+
|                                Application Layer                               |
|--------------------------------------------------------------------------------|
| • Service Catalog / Record Producer                                            |
| • Forms & List Views                                                           |
| • UI Policies                                                                  |
| • Client Scripts                                                               |
| • Access Control (ACLs)                                                        |
+-----------------------------------+--------------------------------------------+
                                    |
                                    v
+--------------------------------------------------------------------------------+
|                               Business Logic Layer                             |
|--------------------------------------------------------------------------------|
| • Flow Designer                                                                |
| • Business Rules                                                               |
| • Script Includes                                                              |
| • Notifications (Email)                                                        |
| • Approval Workflow (Optional)                                                 |
+-----------------------------------+--------------------------------------------+
                                    |
                                    v
+--------------------------------------------------------------------------------+
|                                   Data Layer                                   |
|--------------------------------------------------------------------------------|
| Booking Table                                                                  |
| Driver Table                                                                   |
| Vehicle Table                                                                  |
| User Table (sys_user)                                                          |
+-----------------------------------+--------------------------------------------+
                                    |
                                    v
+--------------------------------------------------------------------------------+
|                             ServiceNow Database                                |
|--------------------------------------------------------------------------------|
| Stores Booking, Driver, Vehicle, User and Workflow Data                        |
+--------------------------------------------------------------------------------+
Architecture Workflow

Employee
    │
    ▼
Submit Cab Booking Request
    │
    ▼
Booking Record Created
    │
    ▼
Flow Designer Triggered
    │
    ▼
Business Rules Execute
    │
    ▼
Driver & Vehicle Assigned
    │
    ▼
Email Notification Sent
    │
    ▼
Ride Started
    │
    ▼
Ride Completed
    │
    ▼
Booking Closed
