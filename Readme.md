# Airline Reservation System (ARS)

## Introduction
The Airline Reservation System (ARS) is an essential software application designed to facilitate the management of airline operations, including:
- Flight scheduling
- Passenger registration
- Booking and cancellation of tickets
- Ticket generation
- Baggage handling  

As the airline industry continues to grow, the need for an efficient and user-friendly system becomes increasingly critical. This project aims to develop a robust ARS that leverages Object-Oriented Programming (OOP) principles to enhance maintainability, scalability, and user experience.

---

## Problem Statement
The current methods of managing airline reservations are often manual and prone to errors, leading to:
- Customer dissatisfaction
- Operational inefficiencies  

Common issues include overbooking, lost baggage, and difficulties in managing flight schedules. Existing systems may also lack an intuitive interface for passengers to book flights or manage their reservations.  

This project seeks to address these challenges by creating a comprehensive ARS that:
- Streamlines the booking process
- Minimizes human error
- Improves overall customer satisfaction

---

## Proposed System
The proposed Airline Reservation System will consist of the following key components:

### **Features:**
1. **Flight Management**  
   - Add, modify, and delete flight details.  

2. **Passenger Registration**  
   - Passengers can register and manage their profiles.  

3. **Booking and Cancellation**  
   - Facilitates booking of tickets and cancellation of existing reservations.  

4. **Ticket Generation**  
   - Generates a digital ticket upon successful booking.  

5. **Baggage Handling**  
   - Tracks baggage allowances and excess baggage fees.  

The system will be **menu-driven**, allowing users to interactively navigate through various functionalities. The core of the system will be built using **OOP principles**, ensuring a modular and extensible design.

---

## OOP Design

### **Classes and Their Functionalities**

1. **Flight**
   - **Attributes**: `flightNumber`, `origin`, `destination`, `departureTime`, `arrivalTime`, `availableSeats`
   - **Functions**:
     - `scheduleFlight()`: Schedule a new flight.
     - `modifyFlight()`: Modify existing flight details.
     - `cancelFlight()`: Cancel a scheduled flight.

2. **Passenger**
   - **Attributes**: `passengerID`, `name`, `email`, `phone`, `baggageAllowance`
   - **Functions**:
     - `register()`: Register a new passenger.
     - `updateProfile()`: Update passenger details.
     - `viewProfile()`: View passenger information.

3. **Booking**
   - **Attributes**: `bookingID`, `passenger`, `flight`, `bookingDate`, `status`
   - **Functions**:
     - `createBooking()`: Create a new booking.
     - `cancelBooking()`: Cancel an existing booking.
     - `viewBookingDetails()`: View booking details.

4. **Ticket**
   - **Attributes**: `ticketID`, `booking`, `issueDate`, `ticketStatus`
   - **Functions**:
     - `generateTicket()`: Generate a ticket for a booking.
     - `validateTicket()`: Validate the ticket status.
     - `reissueTicket()`: Reissue a ticket if needed.

5. **Airport (Composition)**
   - **Attributes**: `airportCode`, `name`, `location`, `flights`
   - **Functions**:
     - `addFlight()`: Add a flight to the airport.
     - `removeFlight()`: Remove a flight from the airport.
     - `listFlights()`: List all flights operating from the airport.

---

### **Additional OOP Features**

1. **Inheritance**
   - The `Passenger` class could be extended to create specialized passenger types, such as `FrequentFlyer` or `VIPPassenger`, with additional attributes like loyalty points or special privileges.

2. **Friend Functions**
   - The `Booking` class may implement friend functions to access private attributes of the `Flight` class, enabling seamless operations like checking available seats during booking.

---

## Interactive Menu-Driven Program
The system will feature a console-based interactive menu to perform the following actions:

### **Flight Management**
- Schedule a Flight
- Modify a Flight
- Cancel a Flight

### **Passenger Management**
- Register as a Passenger
- Update Passenger Profile
- View Passenger Profile

### **Booking Management**
- Create a Booking
- Cancel a Booking
- View Booking Details

### **Ticket Management**
- Generate a Ticket
- Validate a Ticket
- Reissue a Ticket

### **Airport Management**
- Add a Flight to the Airport
- Remove a Flight from the Airport
- List All Flights from the Airport

Each menu option will call the corresponding functions in the classes, facilitating seamless interaction with the system.

---

## Conclusion
The Airline Reservation System aims to provide a comprehensive solution to the challenges faced by the airline industry in managing reservations. With features designed to enhance user experience, streamline operations, and reduce errors, the ARS leverages OOP principles to ensure maintainability and scalability.
