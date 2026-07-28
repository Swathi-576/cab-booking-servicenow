Software Requirements Specification (SRS)

Project Title:
Cab Booking Management System using ServiceNow

Version:
1.0

Prepared By:
Swathi Rokkala

Date:
July 2026

------------------------------------------------------------
1. Introduction
------------------------------------------------------------

1.1 Purpose

The purpose of the Cab Booking Management System is to automate the cab booking process for employees using the ServiceNow platform. The application enables employees to request cabs, administrators to assign drivers and vehicles, and drivers to manage assigned trips efficiently.

1.2 Scope

The system provides a centralized platform to:

• Submit cab booking requests
• Assign drivers and vehicles
• Track booking status
• Manage ride completion
• Generate reports and dashboards
• Send booking notifications

1.3 Intended Users

• Employees
• Drivers
• Transport Administrators
• System Administrators

------------------------------------------------------------
2. Overall Description
------------------------------------------------------------

2.1 Product Perspective

The Cab Booking Management System is a custom ServiceNow application developed using:

• App Engine Studio
• Flow Designer
• Business Rules
• Client Scripts
• UI Policies
• Reports and Dashboards

2.2 Product Features

• User Authentication
• Cab Booking
• Driver Management
• Vehicle Management
• Booking Approval (Optional)
• Ride Tracking
• Booking History
• Notifications
• Reports

------------------------------------------------------------
3. Functional Requirements
------------------------------------------------------------

FR-1 User Login

The system shall allow authorized users to log in.

FR-2 Cab Booking

Employees shall be able to create new cab booking requests.

FR-3 Driver Assignment

Transport administrators shall assign available drivers.

FR-4 Vehicle Assignment

Transport administrators shall assign available vehicles.

FR-5 Booking Status

The system shall maintain booking status.

Status values include:

• Requested
• Assigned
• In Progress
• Completed
• Cancelled

FR-6 Notifications

The system shall notify employees when:

• Booking is created
• Driver is assigned
• Ride is completed
• Booking is cancelled

FR-7 Reports

The system shall generate booking reports.

------------------------------------------------------------
4. Non-Functional Requirements
------------------------------------------------------------

Performance

The system shall process booking requests efficiently.

Availability

The application shall be available to authorized users whenever the ServiceNow instance is available.

Security

• Role-based access control
• Secure authentication
• Access Control Lists (ACLs)

Reliability

The system shall maintain accurate booking records.

Usability

The application shall provide simple and user-friendly forms.

------------------------------------------------------------
5. Database Requirements
------------------------------------------------------------

Tables

1. Booking
2. Driver
3. Vehicle

Booking Fields

• Booking Number
• Employee
• Pickup Location
• Destination
• Pickup Date
• Vehicle Type
• Driver
• Vehicle
• Fare
• Status

Driver Fields

• Driver Name
• Phone Number
• License Number
• Availability

Vehicle Fields

• Vehicle Number
• Vehicle Type
• Capacity
• Availability

------------------------------------------------------------
6. Business Rules
------------------------------------------------------------

• Auto-generate booking number
• Prevent duplicate bookings
• Validate pickup date
• Update driver availability
• Update vehicle availability
• Close booking after ride completion

------------------------------------------------------------
7. Workflow
------------------------------------------------------------

Employee

↓

Submit Booking

↓

Booking Created

↓

Assign Driver

↓

Assign Vehicle

↓

Ride Started

↓

Ride Completed

↓

Booking Closed

------------------------------------------------------------
8. User Roles
------------------------------------------------------------

Employee

• Create booking
• View own bookings
• Cancel booking

Driver

• View assigned bookings
• Update ride status

Transport Admin

• Manage bookings
• Manage drivers
• Manage vehicles
• View reports

------------------------------------------------------------
9. Assumptions
------------------------------------------------------------

• All employees are registered users.
• Drivers are available before assignment.
• Vehicles are maintained by the transport administrator.

------------------------------------------------------------
10. Future Enhancements
------------------------------------------------------------

• Google Maps integration
• Live GPS tracking
• Mobile application
• QR code ride verification
• Payment integration
• Email and SMS notifications

------------------------------------------------------------
11. Conclusion
------------------------------------------------------------

The Cab Booking Management System improves the efficiency of transport management by automating booking, driver assignment, ride tracking, and reporting through the ServiceNow platform.
