Here’s the user stories formatted in **Markdown** for easy reference:

---

# **User Stories for QR Code-based Attendance System**

## **Roles**

### **1. Administrator**
As an administrator, I want to manage employees, attendance, and system settings efficiently.

#### **Employee Management**
- **Add Employee Details**
  - As an admin, I want to add an employee's name, department, teaching hours, and photo so that their information is stored in the system.
  - **Acceptance Criteria:**
    - A form to input employee details.
    - The ability to upload and save employee photos.
    - Successful confirmation after saving.

- **Generate Unique QR Code for Each Employee**
  - As an admin, I want the system to automatically generate a unique QR code for each employee based on their details so they can use it for attendance.
  - **Acceptance Criteria:**
    - QR code is generated after employee registration.
    - Option to view, print, or download the QR code.

- **View Employee List**
  - As an admin, I want to view a list of all employees with their details and QR codes so that I can manage them easily.
  - **Acceptance Criteria:**
    - Table displaying employee names, departments, teaching hours, and a QR code icon.
    - Search and filter options by department or name.

- **Edit Employee Details**
  - As an admin, I want to update an employee’s details (name, department, teaching hours, or photo) so their information remains accurate.
  - **Acceptance Criteria:**
    - Edit form with pre-filled current data.
    - Successful confirmation after saving changes.

- **Delete Employee**
  - As an admin, I want to delete an employee's record (and QR code) if they leave the organization.
  - **Acceptance Criteria:**
    - Confirmation dialog before deletion.
    - Removal of employee record and QR code from the system.

#### **Attendance Management**
- **View Attendance Logs**
  - As an admin, I want to view attendance logs for all employees to monitor time-in and time-out records.
  - **Acceptance Criteria:**
    - Table showing employee name, date, time-in, and time-out.
    - Filter options by date, department, or employee name.

- **Export Attendance Reports**
  - As an admin, I want to export attendance logs to Excel or PDF for payroll and record-keeping.
  - **Acceptance Criteria:**
    - Button to export filtered data.
    - Export includes all relevant columns (employee name, date, time-in, time-out, etc.).

- **Correct Attendance Records**
  - As an admin, I want to manually adjust attendance logs in case of errors (e.g., missed clock-out).
  - **Acceptance Criteria:**
    - Editable fields for time-in and time-out in attendance logs.
    - Confirmation message after changes.

#### **System Settings**
- **Manage Webcam Scanner**
  - As an admin, I want to test and configure the webcam for QR code scanning to ensure it works properly.
  - **Acceptance Criteria:**
    - Test mode to preview webcam feed.
    - Notifications for scanner status (working or error).

- **Set Attendance Rules**
  - As an admin, I want to define attendance rules (e.g., allowable time-in range) to prevent misuse.
  - **Acceptance Criteria:**
    - Settings for time-in and time-out windows (e.g., 8:00 AM to 9:00 AM for clock-in).
    - Warnings for entries outside the allowed time range.

- **Dashboard Overview**
  - As an admin, I want a dashboard with key attendance metrics (e.g., total employees present today, late arrivals, absentees) to get a quick overview.
  - **Acceptance Criteria:**
    - Cards or charts showing daily attendance statistics.
    - Links to detailed logs and reports.

---

### **2. Employee**
As an employee, I want to use my QR code for seamless attendance tracking.

#### **Attendance Logging**
- **Scan QR Code for Time In/Time Out**
  - As an employee, I want to scan my QR code at the webcam to log my time-in or time-out so that my attendance is recorded automatically.
  - **Acceptance Criteria:**
    - Successful scan shows a message: "Time In recorded at [time]" or "Time Out recorded at [time]."
    - Error messages for invalid QR codes or duplicate scans.

- **View Personal Attendance History**
  - As an employee, I want to view my attendance history to check my time-in, time-out, and total hours worked.
  - **Acceptance Criteria:**
    - Table showing personal attendance logs.
    - Filter options by date.

---

### **3. System**
The system should handle all backend processing for secure and accurate attendance management.

#### **Backend Features**
- **Decode QR Code Data**
  - As a system, I want to decode the scanned QR code to extract the employee's unique ID so that I can identify who is logging attendance.
  - **Acceptance Criteria:**
    - Proper decoding of valid QR codes.
    - Error handling for invalid or tampered QR codes.

- **Determine Time In/Out**
  - As a system, I want to determine whether the scan is for a time-in or time-out so that attendance is logged correctly.
  - **Acceptance Criteria:**
    - Logs "Time In" if no previous record exists for the day.
    - Logs "Time Out" if a "Time In" exists for the day.

- **Prevent Duplicate Scans**
  - As a system, I want to reject duplicate time-in or time-out scans for the same employee to ensure data integrity.
  - **Acceptance Criteria:**
    - Rejects scans that attempt to log a second time-in or time-out for the same employee on the same day.

- **Store Attendance Records**
  - As a system, I want to securely store all attendance data in the database so that it can be retrieved for reporting and monitoring.
  - **Acceptance Criteria:**
    - Each log includes employee ID, date, time-in, and time-out.
    - Records are timestamped and linked to the correct employee.

- **Generate Reports**
  - As a system, I want to generate attendance reports in Excel or PDF format so that administrators can easily review records.
  - **Acceptance Criteria:**
    - Generated reports match the filters applied by the admin.
    - Files are downloadable and correctly formatted.

---

## **Summary of Features by Role**

### **Administrator**
- Manage employees (add, edit, delete).
- Generate and manage QR codes.
- View/export attendance logs.
- Configure attendance rules.
- View dashboard metrics.

### **Employee**
- Scan QR code for time-in and time-out.
- View personal attendance history.

### **System**
- Decode QR codes and identify employees.
- Log time-in and time-out securely.
- Prevent duplicate scans.
- Store data securely.
- Generate attendance reports.

---

Let me know if you’d like me to expand on any of these stories or prioritize specific features!
