# Hostel Information System

This project is a comprehensive Hostel Information System (HIS) designed to efficiently manage and organize hostel facilities and operations. HIS primarily focuses on providing access to information for stakeholders such as hostel administrators, students, parents, and staff members.

## Features

- **Student Information Management**: Manage student details, including enrollment and personal information.
- **Room Allocation**: Efficiently allocate rooms to students based on availability and requirements.
- **Fee Management**: Track and manage hostel fees and payments.
- **In-Charge and Warden Management**: Manage the details and roles of in-charges and wardens.
- **Reporting**: Generate insightful reports on hostel operations, occupancy rates, and fee collections.

## Technologies Used

- **Database**: Microsoft Access
- **GUI and Reporting**: Access forms and reports

## Database Schema

The database schema includes the following tables:

- **STUDENT**: Stores student information (s_id, s_name, sem, sec, h_id, mentor_name, age, s_branch, phone).
- **HOSTEL**: Stores hostel details (h_name, h_id, head_warden, build_time, type).
- **ROOMS**: Manages room details (h_id, bed_no, fees, washroom_attach, AC, type).
- **IN-CHARGE**: Stores in-charge details (h_id, join_date, address, i_name, i_id).
- **WARDEN**: Manages warden information (location, phone, grade, emp_no, i_id, emp_name).

## Relationships

- **STUDENT** stays in **HOSTEL** (Many-to-One).
- **HOSTEL** has many types of **ROOMS** (One-to-Many).
- A **HOSTEL** is assigned to an **IN-CHARGE** (One-to-One).
- **IN-CHARGE** manages the **WARDENS** (One-to-Many).

## How to Use

1. **Open the database**:
    - Open the provided Access database file `Hostel Management.accdb` in Microsoft Access.
2. **Navigate through the system**:
    - Use the forms provided to input and manage data.
    - Generate reports using the predefined report templates to get insights into hostel management.
