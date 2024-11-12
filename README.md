# Deluxe Hotel Reservations System 

## Overview

The **Deluxe Hotel Reservations System** project is designed to modernize the operations of a fast-growing hotel in Botswana by automating the reservations and booking processes. This case study is part of the **System Development Life Cycle (SDLC)** and includes planning, analysis, design, and implementation phases. The goal is to develop a web-based application that improves operational efficiency, enhances user experience, and supports customer engagement for hotel reservations.

The project will be developed in phases, starting with the planning and analysis of requirements, followed by system design and the initial steps of the implementation.

---

## Project Phases

The project follows the **System Development Life Cycle (SDLC)** methodology:

### 1. **Planning** 
The planning phase includes an evaluation of the project's **feasibility** in four critical areas:
- **Technical Feasibility**: Assessing the hardware, software, and network requirements to support the system.
- **Economic Feasibility**: Determining the cost-effectiveness of the project, including the expected ROI.
- **Schedule Feasibility**: Ensuring the project can be delivered within the proposed timeline.
- **Operational Feasibility**: Analyzing how the system will fit into the current operations of the hotel and how it can improve existing processes.

### 2. **Analysis** 
The analysis phase identifies detailed system requirements, such as:
- **Request for Proposal (RFP)**: A document outlining the scope, objectives, and expectations for the new system.
- **Functional Requirements**: Specific features the system must support, like room reservation, booking confirmations, and customer management.
- **Non-Functional Requirements**: Key system characteristics such as accessibility, security, and scalability.

### 3. **Design** 
This phase includes the creation of various system models:
- **Functional Model**: Use case diagrams that define the interactions between users and the system.
  ![Use Case Diagram]()  
  *(Click to view the full use case diagram)*

- **Structural Model**: Class diagrams to describe the relationships between system components and the underlying data.
  ![Class Diagram](docs/diagrams/class_diagram.png)  
  *(Click to view the full class diagram)*
  
- **Behavioral Model**: Activity and sequence diagrams that describe how the system processes data and handles user interactions.
  ![Activity Diagram](docs/diagrams/activity_diagram.png)  
  *(Click to view the full activity diagram)*  
  ![Sequence Diagram](docs/diagrams/sequence_diagram.png)  
  *(Click to view the full sequence diagram)*

### 4. **Implementation** 
In this stage, the system's architecture is defined, and core features are outlined:
- **Flowchart**: A visual representation of the system's booking logic, from room selection to payment processing.
  **Flowchart**: A visual representation of the system's booking logic, from room selection to payment processing.  
  ![Flowchart](docs/diagrams/flowchart.png)  
  *(Click to view the full flowchart)*
  
- **Pseudocode**: A step-by-step breakdown of the system's booking logic, outlining how data will be processed and validated.

### 5. **Review** 
The review phase includes project management tasks, such as:
- Completing the **New Software Table** to identify task dependencies and milestones.
- Drawing a **network diagram** to visualize project dependencies, deadlines, and resource allocation.

---

## Technologies Used

- **Programming Languages**: [Insert programming languages you used, e.g., Python, Java, JavaScript, PHP, etc.]
- **Database**: [Insert database system used, e.g., MySQL, PostgreSQL, MongoDB, etc.]
- **Frameworks/Tools**: [List frameworks, libraries, or tools used, e.g., Django, Flask, React, Laravel, etc.]
- **Version Control**: Git, GitHub
- **Project Management Tools**: [Insert tools, e.g., Microsoft Project, Trello, JIRA, etc.]
- **Diagramming Tools**: [Insert any tools used for UML or flowcharting, e.g., Lucidchart, Draw.io]

---

## Project Outcomes and Next Steps

- The **system design** phase has been completed, and we are now preparing for **implementation**.
- The next step involves translating the system design into working code, including the booking system's core functionality.
- **Testing and Deployment**: Once development is completed, extensive testing will be carried out to ensure the system meets all functional and non-functional requirements before deployment.

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

## Conclusion

This project provides a comprehensive approach to developing a hotel reservation system, addressing all aspects from initial feasibility studies to detailed system design. By following the SDLC approach, this case study demonstrates how to analyze business needs, design technical solutions, and plan for successful implementation.

---
## Contact Information
- **Email**: dmmolotsa@gmail.com

---

## Additional Documentation
For full project details, including diagrams and detailed analysis, refer to the accompanying Word document: *Deluxe_Hotel_Project_Documentation.docx*.

