# Hotel-Management
This C++ program simulates a basic hotel management system with functionalities for room management, customer check-in, check-out, and summary reporting. The code is organized into different classes for customers, rooms, and hotel management.

### Key Components:

1. **Customer Class**:
   - Stores customer information like name, address, phone, booking dates, payment advance, and booking ID.
   
2. **Room Class**:
   - Manages room information including room number, type (AC/Non-AC, comfort level, and size), rent, status (reserved/available), and customer details.
   - Methods:
     - `addRoom`: Adds a new room with details like AC type, comfort level, size, and rent.
     - `searchRoom`: Searches for a room based on its number and displays the room's availability and details.
     - `displayRoom`: Displays the details of a specific room.

3. **Hotel Management (HotelMgnt) Class**:
   - Manages overall hotel operations, including customer check-in, check-out, room availability, and guest summary reports.
   - Inherits from the `Room` class.
   - Methods:
     - `checkIn`: Handles the check-in process for a customer by asking for booking details and updating room status.
     - `getAvailRoom`: Lists all available rooms along with their details.
     - `searchCustomer`: Finds a customer by name and displays the room they have booked.
     - `checkOut`: Calculates the final bill based on the number of days the room was occupied, displays checkout details, and marks the room as available.
     - `guestSummaryReport`: Lists all current guests staying in the hotel and their details.

4. **Global Variables**:
   - `rooms[max]`: An array to store the list of rooms.
   - `count`: Keeps track of the total number of rooms.

5. **Functions**:
   - `manageRooms`: Allows for adding new rooms or searching for an existing room.
   
6. **Main Function**:
   - The main menu offers options to manage rooms, check-in, view available rooms, search for customers, check out, and view guest summary reports.
   - Initializes some pre-configured rooms upon the first run and loops until the user chooses to exit.

Features:
- Room Management: Add and search for rooms.
- Customer Check-In and Check-Out: Book and release rooms for customers, generating bills during checkout.
- Room Availability: View available rooms and guest details.
- File Handling: Checkout details are stored in a file `CheckOut.txt`.

The system is interactive and allows for managing multiple rooms and customers effectively.
