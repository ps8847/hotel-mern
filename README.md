# Introduction 

Welcome to TravelHub – Your Ultimate Destination for Seamless Travel Experiences! 🌍✨

TravelHub is a cutting-edge application built on the MERN (MongoDB, Express.js, React.js, Node.js) stack with TypeScript, designed to revolutionize the way users book hotels and vendors manage their accommodations. Whether you're a traveler seeking the perfect stay or a hotel owner looking to showcase your property, TravelHub is your one-stop solution.

## Key Features:

# User-Friendly Booking System:
Easily search and book hotels based on your preferences. With an intuitive user interface, our app ensures a smooth and hassle-free booking experience. Filter results based on location, amenities, and price range to find the perfect accommodation tailored to your needs.

# Vendor Registration and Management:
Hotel owners and vendors can seamlessly register their properties on TravelHub. Our platform provides a user-friendly dashboard to manage room availability, update pricing, and showcase the unique features of each hotel. Gain visibility in the travel market and attract more guests to your establishment.

# Secure User Authentication:
TravelHub prioritizes the security of user data. Through robust authentication and authorization mechanisms, we ensure that both travelers and vendors have a secure and trustworthy environment for their interactions.

# Real-Time Updates:
Stay informed with real-time updates on booking status, available rooms, and reservation confirmations. Travelers receive instant notifications, while vendors can manage their inventory efficiently, ensuring a seamless flow of information.

# Interactive Maps:
Explore the surrounding areas of hotels through interactive maps integrated into the app. Get a sense of the neighborhood and plan your stay with confidence.

# Responsive Design:
Whether you're accessing TravelHub from your desktop, tablet, or smartphone, our app provides a responsive design, ensuring a consistent and user-friendly experience across all devices.

TravelHub is not just an app; it's a platform that connects travelers with exceptional accommodations and empowers vendors to showcase their properties to a global audience. Join us in creating a world where travel is not just a journey but an unforgettable experience. Download TravelHub today and embark on your next adventure with confidence! 🌟🏨

# Setting Up the MERN Stack Hotel Booking App

This guide will walk you through the process of setting up the PrinceBookings App on your local machine.

## Cloning the Repository

Start by cloning the repository to your local machine:

```bash
git clone https://github.com/ps8847/hotel-mern.git
cd hotel-mern
```

## Backend Configuration

1. **Environment Files**: Navigate to the `backend` folder and create a file `.env` . Add the following contents to the file:

    ```plaintext
    MONGODB_CONNECTION_STRING=

    JWT_SECRET_KEY=
    FRONTEND_URL=

    # Cloudinary Variables
    CLOUDINARY_CLOUD_NAME=
    CLOUDINARY_API_KEY=
    CLOUDINARY_API_SECRET=

    # Stripe
    STRIPE_API_KEY=
    ```

2. **MongoDB Setup**: 
    - Sign up for an account at [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).
    - Create a new cluster and follow the instructions to set up a new database.
    - Once set up, obtain your MongoDB connection string and add it to the `MONGODB_CONNECTION_STRING` variable in your `.env` files.

3. **Cloudinary Setup**:
    - Create an account at [Cloudinary](https://cloudinary.com/).
    - Navigate to your dashboard to find your cloud name, API key, and API secret.
    - Add these details to the respective `CLOUDINARY_*` variables in your `.env` files.

4. **Stripe Setup**:
    - Sign up for a Stripe account at [Stripe](https://stripe.com/).
    - Find your API keys in the Stripe dashboard.
    - Add your Stripe API key to the `STRIPE_API_KEY` variable in your `.env` files.
  
5. **JWT_SECRET_KEY**:
    - This just needs to be any long, random string. You can google "secret key generator".

7. **Frontend URL**:
    - The `FRONTEND_URL` should point to the URL where your frontend application is running (typically `http://localhost:5174/` if you're running it locally).
  

## Frontend Configuration

1. **Environment Files**: Navigate to the `frontend` folder and create a file: `.env`:

    ```plaintext
    VITE_API_BASE_URL=
    VITE_STRIPE_PUB_KEY=
    ```

5. **VITE_API_BASE_URLL**:
    - The `VITE_API_BASE_URL` should point to the URL where your backend application is running (typically `http://localhost:7000` if you're running it locally).

## Running the Application

1. **Backend**:
    - Navigate to the `backend` directory.
    - Install dependencies: `npm install`.
    - Start the server: `npm run dev`.

2. **Frontend**:
    - Open a new terminal and navigate to the `frontend` directory.
    - Install dependencies: `npm install`.
    - Start the frontend application: `npm run dev`.
    - The application should now be running on `http://localhost:5174/` but verify this in your command line terminal  

