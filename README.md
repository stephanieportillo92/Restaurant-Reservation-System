# Restaurant-Reservation-System
Restaurant reservation application - COSC 6342 - Software Engineering Project Management
## System Features

This restaurant reservation system implements all the required features:

1. **User Types**:
  - Supports both guest users and registered users
  - Allows guests to make reservations without logging in
  - Provides optional registration for guest users

2. **Table Search & Reservation**:
  - Users can search for available tables by date, time, and party size
  - Collects name, phone, email, and special requests

3. **Table Capacity Management**:
  - Tables have maximum capacity limits (2, 4, 6, 8)
  - System can combine tables to accommodate larger parties
  - Notifies staff when tables need to be combined

4. **Registered User Features**:
  - Stores user profile with name, addresses, and preferred payment method
  - Tracks Preferred Diner number and earned points
  - Manages payment preferences (cash, credit)

5. **High-Traffic Day Handling**:
  - Identifies high-traffic days that require holding fees
  - Collects credit card information for these reservations
  - Notifies users about the $10 no-show charge policy

6. **User Experience**:
  - Clean, intuitive interface with step-by-step reservation process
  - Confirmation page with reservation details
  - Profile management for registered users


The system is built with Next.js and uses server actions for data processing, making it scalable and maintainable.

## How To Use

To clone and run this application, you'll need [Git](https://git-scm.com), [Node.js](https://nodejs.org/en/download/)
```bash
# Clone this repository
git clone [https://github.com/stephanieportillo92/Restaurant-Reservation-System]
# Go into the repository
Restaurant-Reservation-System

## Credits

This software uses the following open source packages:

- [Node.js](https://nodejs.org/)
