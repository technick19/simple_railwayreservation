# simple_railwayreservation
This Java code represents a simple railway reservation system with functionality for both administrators and users. Here's an explanation of the code:

1. **Classes**: The code defines several classes to model different entities within the railway reservation system:

   - `User`: Represents user information.
   - `ApprovalUser`: Represents user information pending approval.
   - `Train`: Represents train details, including the train name, starting point, destination, number of stations, available seats, station names, and seat allocation.
   - `waitingList`: Represents a waiting list for passengers when all seats are booked.

2. **Static Variables**:
   - `trains`: An ArrayList to store train objects.
   - `user`: An ArrayList to store user objects.
   - `appUser`: An ArrayList to store user objects pending approval.
   - `waitingLis`: An ArrayList to store waiting list objects.

3. **Admin Functions**:
   - `approveUser()`: Admins can approve or reject user registration requests. Approved users are added to the `user` list, while rejected requests are removed from `appUser`.
   - `addTrain()`: Admins can add train details to the system.
   - `decSeat()`: Admins can declare seat availability for a specific train.
   - `trainDetails()`: Admins can view train details, including seat allocation.

4. **User Functions**:
   - `availTic()`: Calculates the number of available tickets for a given train and journey.
   - `allotTicket()`: Allots tickets to users based on seat availability.
   - `WaitingLisAllot()`: Allots tickets for passengers on the waiting list.
   - `userSignup()`: Allows users to sign up for the system, with their details pending admin approval.
   - `userSigning()`: Allows registered users to sign in and access user-specific functions.
   - `UserFunction()`: Provides a menu of user-specific actions.
   - `viewTrains()`: Displays available trains and their details.
   - `bookTicket()`: Allows users to book tickets for a specific train.
   - `ticketCancel()`: Allows users to cancel their booked tickets.

5. **Admin and User Entry Points**:
   - `admin()`: Entry point for admin functionality, including user approval, train addition, seat declaration, and viewing train details.
   - `user()`: Entry point for user functionality, including signing up and signing in.

6. **Main Method**: The `main` method initializes the system with a sample user and train, and it provides a menu for selecting between admin and user actions.

The code implements a basic railway reservation system, allowing administrators to manage trains and users, and users to view trains and book tickets. It also includes a waiting list feature for cases where all seats are booked.
