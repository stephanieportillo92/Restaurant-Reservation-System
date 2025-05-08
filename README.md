# Restaurant-Reservation-System
Restaurant reservation application - COSC 6342 - Software Engineering Project Management
## System Features

This restaurant reservation system implements all the required features:

**User Types**
  - Supports both guest users and registered users
  - Optional registration during reservation process
  - Registered user profiles with all required fields

**Reservation Flow**
  - Search for tables by location, date, time, and party size
  - Table availability display with visual layout
  - Table combination logic for accommodating larger parties
  - Special requests and dietary preferences

**High-Traffic Day Handling**
  - Detection of high-traffic days (holidays, weekends)
  - Credit card holding fee requirement
  - No-show policy notification ($10 charge)

**User Profiles**
  - Name, mailing address, billing address
  - System-generated Preferred Diner number
  - Points tracking (1 point per $1 spent)
  - Preferred payment method selection

**Additional Features**
  - Calendar integration for reservations
  - Waitlist options when desired times are unavailable
  - Reservation modification and cancellation
  - Email confirmation and reminders
  - Visual table layout


### Assumptions Made

1. **Location Awareness**: Implemented location selection upfront in the reservation process
2. **Visual Table Layout**: Created a visual representation of the restaurant floor plan
3. **Wait List Options**: Added functionality to join a waitlist if desired time is unavailable
4. **Special Requests**: Included a field for special requests during reservation
5. **Calendar Integration**: Added Google Calendar integration for reservations
6. **Reminders**: System sends confirmation emails with reservation details
7. **Clear Policy Information**: High-traffic day policies are clearly displayed
8. **User Preferences**: System stores and remembers user preferences


The system is designed to be user-friendly while meeting all the business requirements for the restaurant chain.
The system is built with Next.js and uses server actions for data processing, making it scalable and maintainable.


## Project Description

This is a comprehensive restaurant reservation system for a restaurant chain that allows both guest and registered users to search for and reserve tables. The system includes features such as:

- Table search and reservation for both guest and registered users
- Smart table combination for accommodating different party sizes
- High-traffic day detection with holding fee requirements
- User registration and loyalty program with points tracking
- Visual table layout representation
- Calendar integration for reservations
- Waitlist functionality for unavailable times
- Special requests handling


The application is built using Next.js with the App Router, Tailwind CSS for styling, and shadcn/ui components for the UI elements. It's designed to be responsive and user-friendly across all devices.

## How to Run the Code

### Prerequisites

- Node.js (v16 or later)
- npm or yarn


### Step-by-Step Instructions

1. **Clone the repository**

```shellscript
git clone [repository-url]
cd restaurant-reservation-system
```


2. **Install dependencies**

```shellscript
npm install
# or
yarn install
```


3. **Run the development server**

```shellscript
npm run dev
# or
yarn dev
```


4. **Open your browser**
Navigate to [http://localhost:3000](http://localhost:3000) to see the application running.


## Example User Flow

### Making a Reservation as a Guest User

1. On the homepage, use the reservation search form to:

1. Select a location (e.g., "New York")
2. Choose a date (e.g., "June 15, 2025")
3. Select a time (e.g., "19:00")
4. Specify party size (e.g., "4 people")



2. Click "Find a Table" to see available tables.
3. On the available tables page:

1. View table options (single tables or combinations)
2. Select your preferred table arrangement
3. Click "Reserve Selected Table"



4. On the reservation details page:

1. Fill in your contact information (name, phone, email)
2. Add any special requests
3. Optionally check the box to create an account
4. If it's a high-traffic day, provide payment information
5. Click "Complete Reservation"



5. View your reservation confirmation with details and options to:

1. Add to calendar
2. Share reservation details
3. Modify or cancel the reservation





### Registering as a User

1. Click "Sign Up" in the navigation bar.
2. Fill in the registration form with:

1. Personal information (name, phone, email, password)
2. Address information
3. Payment preferences
4. Agree to terms and conditions



3. Click "Create Account" to complete registration.
4. You'll receive a Preferred Diner number and can start earning points with reservations.


## Special Features

### High-Traffic Day Detection

The system automatically detects high-traffic days such as:

- Weekends (Friday and Saturday)
- Holidays (New Year's, Valentine's Day, Mother's Day, etc.)
- Special occasions


On these days, users are required to provide credit card information to hold the reservation, with a $10 charge for no-shows.

### Table Combination Logic

When a table for the exact party size isn't available, the system intelligently suggests combinations:

- For a party of 8, it might suggest two tables of 4
- For a party of 6, it might suggest a table of 4 and a table of 2


The system notifies the restaurant staff that tables need to be combined.

### Loyalty Program

Registered users earn 1 point for every $1 spent at the restaurant. These points can be redeemed for discounts and special offers.

## Special Setup Instructions

This project doesn't require any special setup beyond the standard Next.js development environment. All data is currently mocked within the application for demonstration purposes.

In a production environment, you would need to:

1. Connect to a database for storing user information and reservations
2. Implement authentication services
3. Set up email notification services
4. Configure payment processing for high-traffic day reservations


## Note on Data

Currently, the application uses mock data for demonstration purposes. In a production environment, you would need to replace the mock data with actual database calls and API integrations.
