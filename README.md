# Clinic Management System

A role-based clinic management system for coordinating organization administration, patient registration, triage, laboratory requests, and asset tracking in one place.

## Project goal

The system brings clinic departments together around shared records, clear access roles, and connected operational workflows.

This project is designed to handle:

- organization management
- user roles and access control
- patient intake and registration
- triage and request routing
- laboratory workflows
- asset ownership and request handling
- administrative reports and dashboards

## Purpose

Clinic teams need to coordinate patient intake, clinical requests, laboratory work, administration, and inventory. This project provides a central place to manage those workflows, assign responsibilities, and keep track of work across departments.

## System architecture

The project is organized into modules, giving each clinic role or department a dedicated workflow within the wider system.

The project includes:

- PHP backend logic
- MySQL-compatible database structure
- Bootstrap-based UI
- JavaScript and jQuery for interactive pages
- dashboard-style reporting components
- shared CSS, icons, fonts, and image assets

The modular structure keeps the different workflows grouped by function.

## Main modules

### 1. Super admin section
Directory: `supperadminspage/`

This section provides high-level administration, including:

- system-wide user oversight
- organization setup
- user approval and denial
- role-based access control
- platform-level management

### 2. Organization admin section
Directory: `orgadminspage/`

This section manages organization-level operations, including:

- user and office relations
- organization-level settings
- permission control
- role assignment within organizations

### 3. Patient registration section
Directory: `petientreg/`

This module covers patient intake and registration, including:

- patient records
- appointment and registration workflows
- operational record handling
- patient-related administrative tasks

### 4. Triage section
Directory: `triage/`

This module handles incoming requests and their routing, including:

- triage workflow handling
- request acceleration or referral
- early-stage clinical tracking

### 5. Laboratory section
Directory: `labratory/`

This module handles laboratory requests, including:

- test requests
- laboratory intake
- request monitoring
- follow-up and internal routing

### 6. Asset request and issue handling
Directory: `assetrequestissue/`

This module handles internal asset requests and issues, including:

- issue creation
- request tracking
- approval workflows
- transfer or routing between departments

### 7. Asset ownership and stock management
Directory: `assetownerspage/`

This section tracks stored assets and ownership, including:

- asset registration
- inventory management
- ownership status
- request acceptance and fulfillment

### 8. Reporting and office-level analytics
Directory: `haeadoaffice/`

This section provides operational and office-level reports, including:

- office activity reporting
- asset summaries
- department-level insights
- dashboard-style metrics

## Project structure

```text
clinicsystem/
├── assetownerspage/          # asset ownership and storage workflows
├── assetrequestissue/        # requests, issue tracking, and internal routing
├── assets/                   # UI assets, vendor libraries, and shared resources
├── css/                      # stylesheet files
├── db/                       # database files and connection-related assets
├── fonts/                    # font resources
├── haeadoaffice/             # office and asset reporting modules
├── image/                    # static images and visual content
├── js/                       # frontend scripts and interactions
├── labratory/                # lab request workflow screens
├── link/                     # CSS and JS include helpers
├── orgadminspage/            # organization and role management
├── petientreg/               # patient registration and workflow screens
├── serachfile/               # search-related functionality
├── supperadminspage/         # super admin functionality
├── triage/                   # triage and routing screens
└── README.md                 # project documentation
```

## Core workflow

The system connects the main clinic workflows:

1. Super admins manage organizations and user access.
2. Organization admins assign roles and manage internal relationships.
3. Front-desk or registration staff handle patient records.
4. Triage routes requests to the proper department.
5. Laboratory staff process requested tests or analysis.
6. Asset-related requests are tracked and approved.
7. Managers review reports to monitor performance and operations.

Together, these workflows provide a shared operational system for clinic administration and day-to-day work.

## Tech stack

The project uses:

- PHP for server-side logic
- MySQL-compatible database storage
- HTML and CSS for layout and styling
- Bootstrap for responsive admin interface design
- JavaScript and jQuery for interactivity
- Chart.js and dashboard widgets for reporting
- Apache/XAMPP/WAMP-style local setup

## Local setup

The setup below describes a standard local PHP and MySQL environment. Exact configuration may depend on the database scripts and connection settings included with your copy of the project.

### Requirements

- PHP 7+ or newer
- Apache or Nginx
- MySQL or MariaDB
- XAMPP, WAMP, MAMP, or similar local environment
- optional phpMyAdmin for database import

### Setup steps

1. Start your local web server and database service.
2. Import the SQL files into your MySQL database.
3. Update the database connection details in the project config files.
4. Place the project in your web root directory.
5. Open the application through the browser.
6. Log in with the appropriate role-based credentials.

## Database and security notes

Before production use, configure and verify the security measures appropriate for the deployment, including:

- secure password hashing
- prepared statements for SQL queries
- CSRF protection
- session validation
- role-based access enforcement
- input validation and sanitization
- audit logs for critical actions

## Project focus

The system is designed to help clinics stay organized and coordinated by bringing administrative and departmental workflows into a centralized platform. Shared operational visibility helps staff track work and coordinate across departments.

## Future improvements

Potential next steps for the project:

- cleaner modular backend structure
- proper database schema documentation
- complete user role matrix
- better installation and deployment guide
- UI screenshots and user flow documentation
- automated testing for core workflows
- better separation of business logic from templates

## License

No license is currently specified. Add a license before redistributing the project so users know how it may be used.

## Final note

The Clinic Management System brings administrative and operational workflows together in a role-based platform that can be extended as clinic needs grow.
