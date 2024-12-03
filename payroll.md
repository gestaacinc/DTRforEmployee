Here’s your finalized **business rules** in Markdown format:

---

# **Business Rules for Payroll System**

## **Base Salary**
- **Daily Salary:** PHP 1,500.
- **Work Hours:**
  - Expected Time-In: **8:00 AM**.
  - Expected Time-Out: **5:00 PM**.
- **Lunch Break:**
  - Time: **12:00 PM to 1:00 PM**.
  - **Rule:** Unpaid.
- **Payable Hours:** 8 hours per day.
- **Policy:** **No work, no pay.**

---

# Grace Period
- **Duration:** 15 minutes (8:00 AM to 8:15 AM).
- **Rule:** Employees clocking in within the grace period will receive no deductions.
  - **Example:** Clock-in at **8:10 AM** → **No deduction**.

# Deductions for Tardiness

## 1. After Grace Period (Late)
- **Rule:** Deduct based on the minutes late, calculated as:
  \[
  \text{Deduction} = \frac{\text{Minutes Late} \times \text{Hourly Rate}}{60}
  \]
- **Hourly Rate Calculation:**
  \[
  \text{Hourly Rate} = \frac{\text{Daily Salary}}{\text{Payable Hours}} = \frac{1,500}{8} = 187.50 \, \text{PHP/hour}
  \]
- **Example:**
  - Clock-in at **8:20 AM** (5 minutes late):
    \[
    \text{Deduction} = \frac{5 \times 187.50}{60} = 15.63 \, \text{PHP}
    \]

## 2. 1 Hour Late or More
- **Rule:** Deduct based on total hours late (including partial hours).
- **Examples:**
  - **Clock-in at 9:00 AM** (1 hour late):
    \[
    \text{Deduction} = 187.50 \, \text{PHP/hour} = 187.50 \, \text{PHP}
    \]
  - **Clock-in at 9:10 AM** (1 hour and 10 minutes late):
    \[
    \text{Deduction} = 187.50 + \frac{10 \times 187.50}{60} = 218.75 \, \text{PHP}
    \]


---

## **No Clock-In**
- **Rule:** If an employee does not clock in, they receive no salary for the day.
- **Deduction:** Full daily salary (PHP 1,500).
- **Example:**
  - No clock-in → Deduction = **PHP 1,500**.

---

## **Time-Out Handling**
- **Morning:** Work until **12:00 PM**.
- **Afternoon:** Work until **5:00 PM**.
- **Lunch Break:** Always unpaid (12:00 PM to 1:00 PM).
- **Policy:** No deductions for time-out unless there’s a no-clock-in issue for part of the day.

---

## **Summary Table**

| **Event**                   | **Rule**                                                                                     | **Example**                          | **Deduction** | **Total Pay** |
|-----------------------------|-----------------------------------------------------------------------------------------------|--------------------------------------|---------------|---------------|
| **On-Time (8:00 AM)**       | No deductions.                                                                                | Clock-in: 8:00 AM                    | PHP 0         | PHP 1,500     |
| **Grace Period (8:15 AM)**  | No deductions within 15 minutes of start time.                                                | Clock-in: 8:10 AM                    | PHP 0         | PHP 1,500     |
| **Late (8:16 AM - 8:59 AM)**| Deduct based on minutes late (\( \text{Minutes Late} \times \text{Hourly Rate} / 60 \)).       | Clock-in: 8:20 AM (5 mins late)      | PHP 15.63     | PHP 1,484.37  |
| **1 Hour Late (After 9:00)**| Deduct for total hours late (including partial hours).                                         | Clock-in: 9:10 AM                    | PHP 218.75    | PHP 1,281.25  |
| **No Clock-In**             | No work, no pay.                                                                              | No clock-in                          | PHP 1,500.00  | PHP 0         |

---

This Markdown provides a clean and structured explanation of the rules for documentation or further review. Let me know if you’d like to refine anything!
