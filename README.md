# Clinic Management System

I built this project as a role-based clinic management system to help manage hospital and clinic operations from one place. It brings together organization administration, patient registration, triage, laboratory requests, and asset tracking into a single PHP-based web application.

## Project goal

I created this system to support the day-to-day workflow of a clinic environment where different departments need to work together without losing control of records, permissions, or operational flow.

This project is designed to handle:

- organization management
- user roles and access control
- patient intake and registration
- triage and request routing
- laboratory workflows
- asset ownership and request handling
- administrative reports and dashboards

## Why I built it

I wanted a system that could manage the full clinical workflow in one place instead of splitting operations across different tools and disconnected processes. The goal was to make it easier for admins, staff, and department heads to track work, assign responsibilities, and keep the clinic running smoothly.

## System architecture

I structured the project as a modular PHP application so that each section of the clinic has its own workflow while still staying connected to the same overall system.

The project includes:

- PHP backend logic
- MySQL-compatible database structure
- Bootstrap-based UI
- JavaScript and jQuery for interactive pages
- dashboard-style reporting components
- shared CSS, icons, fonts, and image assets

This makes the project easy to manage for a small to medium-sized clinic or healthcare operation.

## Main modules

### 1. Super admin section
Directory: `supperadminspage/`

This part of the system is for high-level administration. It handles:

- system-wide user oversight
- organization setup
- user approval and denial
- role-based access control
- platform-level management

### 2. Organization admin section
Directory: `orgadminspage/`

This section supports internal organization management and helps with:

- user and office relations
- organization-level settings
- permission control
- role assignment within organizations

### 3. Patient registration section
Directory: `petientreg/`

This module is focused on patient intake and registration, including:

- patient records
- appointment and registration workflows
- operational record handling
- patient-related administrative tasks

### 4. Triage section
Directory: `triage/`

This module helps route and prioritize incoming requests. It supports:

- triage workflow handling
- request acceleration or referral
- early-stage clinical tracking

### 5. Laboratory section
Directory: `labratory/`

I built this part to handle lab-related request processing, including:

- test requests
- laboratory intake
- request monitoring
- follow-up and internal routing

### 6. Asset request and issue handling
Directory: `assetrequestissue/`

This module is focused on internal asset and request processes, including:

- issue creation
- request tracking
- approval workflows
- transfer or routing between departments

### 7. Asset ownership and stock management
Directory: `assetownerspage/`

This section helps track stored assets and their ownership, including:

- asset registration
- inventory management
- ownership status
- request acceptance and fulfillment

### 8. Reporting and office-level analytics
Directory: `haeadoaffice/`

This area is built for operational visibility and summary reporting, such as:

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
├── README.md                 # project documentation
├── ._amslast.sql             # SQL snapshot
├── ._assetdb.sql             # database snapshot
├── ._captcha.php             # supporting file from original project snapshot
├── ._index.php               # project entry snapshot
├── ._login.php               # login-related snapshot
└── .git/                     # repository metadata
```

## Core workflow

I designed this project around a complete clinic operations flow:

1. Super admins manage organizations and user access.
2. Organization admins assign roles and manage internal relationships.
3. Front-desk or registration staff handle patient records.
4. Triage routes requests to the proper department.
5. Laboratory staff process requested tests or analysis.
6. Asset-related requests are tracked and approved.
7. Managers review reports to monitor performance and operations.

This makes the system useful as a full operational dashboard for a clinic environment, not just a single feature module.

## Tech stack

I built this project using:

- PHP for server-side logic
- MySQL-compatible database storage
- HTML and CSS for layout and styling
- Bootstrap for responsive admin interface design
- JavaScript and jQuery for interactivity
- Chart.js and dashboard widgets for reporting
- Apache/XAMPP/WAMP-style local setup

## Local setup

This project appears to be a restored snapshot of an older codebase, so the exact setup depends on how the source was extracted and restored.

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

I built this as an internal operational system, so a production-ready version should include:

- secure password hashing
- prepared statements for SQL queries
- CSRF protection
- session validation
- role-based access enforcement
- input validation and sanitization
- audit logs for critical actions

## What I wanted this project to do

I wanted this project to help a clinic stay organized, coordinated, and efficient. The system is meant to reduce manual handling, improve visibility across departments, and make it easier for administrators and staff to work from a centralized platform.

## Future improvements

Some improvements I would still want to add in a production version:

- cleaner modular backend structure
- proper database schema documentation
- complete user role matrix
- better installation and deployment guide
- UI screenshots and user flow documentation
- automated testing for core workflows
- better separation of business logic from templates

## License

This repository does not currently include a declared license file. If I decide to share this project publicly, I would add a proper license such as MIT or Apache 2.0.

## Final note

This project reflects the work I put into building a clinic management platform that covers both administrative and operational needs. It is designed to be practical, role-based, and easy to extend as the system grows.

