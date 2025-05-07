# Restaurant-Reservation-System
Restaurant reservation application - COSC 6342 - Software Engineering Project Management
### Restaurant Reservation System

I'll create a comprehensive restaurant reservation system based on your requirements. This system will handle both guest and registered users, table combinations, high-traffic days with holding fees, and user profiles.

```typescriptreact project="restaurant-reservation"
...
```

## System Features

This restaurant reservation system implements all the required features:

1. **User Types**:

1. Supports both guest users and registered users
2. Allows guests to make reservations without logging in
3. Provides optional registration for guest users



2. **Table Search & Reservation**:

1. Users can search for available tables by date, time, and party size
2. Collects name, phone, email, and special requests



3. **Table Capacity Management**:

1. Tables have maximum capacity limits (2, 4, 6, 8)
2. System can combine tables to accommodate larger parties
3. Notifies staff when tables need to be combined



4. **Registered User Features**:

1. Stores user profile with name, addresses, and preferred payment method
2. Tracks Preferred Diner number and earned points
3. Manages payment preferences (cash, credit, check)



5. **High-Traffic Day Handling**:

1. Identifies high-traffic days that require holding fees
2. Collects credit card information for these reservations
3. Notifies users about the $10 no-show charge policy



6. **User Experience**:

1. Clean, intuitive interface with step-by-step reservation process
2. Confirmation page with reservation details
3. Profile management for registered users





The system is built with Next.js and uses server actions for data processing, making it scalable and maintainable.
