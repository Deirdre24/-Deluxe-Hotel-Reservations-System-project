# Deluxe Hotel Reservations System

## Overview
The Deluxe Hotel Reservations System project provides an automated, web-based solution for hotel reservations, addressing the operational needs of Deluxe Hotel in Botswana. This system helps manage reservations, bookings, and critical customer and staff data, reducing the manual workload and enhancing efficiency. This project was developed to fulfill the requirements of a Systems Development Life Cycle (SDLC) project, covering planning, analysis, design, implementation, and review.

## Objectives
1. Capture and store essential hotel data, including reservations, payments, rooms, and customer details.
2. Facilitate efficient, online reservations and registration.
3. Record and manage customer details, supporting easy reuse for repeat bookings.
4. Ensure secure data access for hotel staff and registered users.
5. Provide real-time room availability and pricing details.
6. Enable room reservations from any location with internet access.

---

## Feasibility Analysis
### 1. Technical Feasibility
Evaluates hardware, software, internet connectivity, and security requirements. Examines the compatibility of the new system with existing infrastructure and assesses integration risks.

### 2. Economic Feasibility
Assesses whether development costs align with budget constraints, focusing on cost-benefit analysis to estimate Return on Investment (ROI) and the payback period.

### 3. Schedule Feasibility
Evaluates whether the project timeline is realistic, ensuring optimal resource allocation within set deadlines.

### 4. Operational Feasibility
Determines the new system’s effectiveness in addressing the hotel’s operational challenges and assesses the adaptability of hotel staff and management.

---

## Request for Proposal (RFP)

### Project Overview
The Deluxe Hotel management requires a solution to replace their manual, paper-based system. This proposal outlines the need for a web-based system to streamline bookings, reduce processing time, prevent data loss, and provide convenient, remote access to hotel services for both customers and staff.

### Project Objectives
1. **System Automation**: Replace manual booking processes with automated, online solutions.
2. **Data Security**: Implement secure access protocols to protect critical hotel information.
3. **User Accessibility**: Enable ease of access to hotel services and booking details for both customers and hotel staff.

### Deliverables
1. Fully functional web-based application.
2. Comprehensive system documentation.
3. Training and support materials for hotel staff.

---

## Requirements

### Functional Requirements
- The system should send reservation and payment confirmation messages.
- Capture and store customer reservation details, such as booking date, check-in, and check-out information.
- Display room rates and apply discounts for qualifying bookings.
- Validate user login credentials.
- Cancel bookings if payment is not received within three days.

### Non-functional Requirements
- **Accessibility**: Accessible through public web pages.
- **Ease of Use**: Simple and intuitive user interface.
- **Security**: Only authorized users can access sensitive information; ensures payment and personal data protection.

---

## System Design

### Use Case & Diagrams
- **Use Case Diagrams**: Visual representation of system functionalities, accessible [here](#).
- **Class Diagrams**: Describes relationships between system classes, accessible [here](#).
- **Activity Diagrams**: Workflow of key activities within the booking and reservation process.
- **Sequence Diagrams**: Details the interaction between objects in the booking process.

---

## Pseudocode Solution

Below is a structured pseudocode example for handling the booking and reservation process:

1. START
2. Declare variables
3. Set discount rate and payment deadline
4. Prompt user for login details
5. Accept reservation details (check-in, check-out dates, room count)
6. Calculate total price with applicable discounts
7. Confirm availability of rooms
8. Process payment or cancel reservation if deadline passes
9. END

## Pseudocode Solution

```plaintext
1. START
2. 
3. //declare variables
4. Date ExpectedCheckInDate, ExpectedCheckoutDate, DateOfBooking
5. Time Time
6. Int NoOfRooms
7. Decimal TotalPrice, DiscountedTotalPrice, Discount
8. Date, Time, Int AvailableRooms, Time, ReservedRooms, DateOfBooking
9. String Reserved, Duration, BookingDetails
10. Int NoOfDays
11. 
12. //Initialise values
13. Discount = 0.1
14. PaymentDeadline = DateOfBooking + 3
15. 
16. PRINT (“Please Enter log in details”)
17. 
18. ExpectedCheckInDate = PRINT(“Please Enter check-in date (DD-MM-YYYY):”)
19. ExpectedCheckOutDate = PRINT(“Please Enter check-out date (DD-MM-YYYY):”)
20. 
21. NoOfDays = ExpectedCheckOutDate – ExpectedCheckInDate
22. 
23. AvailableRooms = get_available_rooms( CheckInDate, CheckOutDate, Time, NoOfRooms)
24. 
25. NoOfRooms = PRINT(“Enter number of rooms needed: “)
26. IF NoOfRooms <= AvailableRooms
27. THEN Reserved = reserve_room(ExpectedCheckInDate, ExpectedCheckOutDate, Time)
28. IF Duration = Weekdays
29. THEN TotalPrice = P350 * NoOfDays
30. IF NoOfDays > 3 
31. THEN DiscountedTotalPrice = TotalPrice * Discount
32. PRINT (“Your Bill is: DiscountedTotalPrice”)
33. ELSE
34. PRINT (“Your Bill is: TotalPrice”)
35. ENDIF
36. ELSEIF Duration = Weekends
37. THEN TotalPrice = P500 * NoOfDays
38. ENDIF  
39. 
40. Function processPayment(BookingDetails, TotalPrice, DiscountedTotalPrice)  
41. As String
42. IF DateOfBooking > PaymentDeadline THEN
43. cancelBooking(Booking)
44. Return (“Reservation Cancelled”)
45. ELSE
46. UpdateBooking(BookingDetails)
47. Return (“paid”)
48. END Function
49. 
50. ELSE
51. PRINT (“Sorry, there are no rooms available”) 
52. ENDIF
53. STOP
```

--- 

## Critical Path Review

| ID  | Task            | Dependence | Expected Time (ET) | Earliest Finish Time (EF) | Latest Finish Time (LF) | Critical Activity |
|-----|------------------|------------|---------------------|----------------------------|--------------------------|-------------------|
| 1   | Requirements     | -          | 10                 | 10                         | 10                       | Yes               |
| 2   | Analysis         | 1          | 8                  | 18                         | 18                       | Yes               |
| 3   | Documentation    | 1          | 15                 | 44                         | 25                       | No                |
| 4   | Logical Design   | 2          | 6                  | 24                         | 24                       | Yes               |
| 5   | Report Design    | 4          | 4                  | 28                         | 29                       | No                |
| 6   | Form Design      | 4          | 5                  | 29                         | 29                       | Yes               |
| 7   | Implementation   | 5,6        | 15                 | 44                         | 44                       | Yes               |
| 8   | Installation     | 3,7        | 3                  | 47                         | 47                       | Yes               |

---

## Project Timeline
- **Project Start Date**: May 1, 2023
- **Due Date**: June 20, 2023
- **Estimated Budget**: P900,000

---

## Contact Information
- **Email**: dmmolotsa@gmail.com

---

## Additional Documentation
For full project details, including diagrams and detailed analysis, refer to the accompanying Word document: *Deluxe_Hotel_Project_Documentation.docx*.

