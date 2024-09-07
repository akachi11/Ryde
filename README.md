# 🚗 Ryde - Uber Clone App

**Ryde** is a simplified Uber clone built with **React Native**, designed to allow users to book rides between selected locations seamlessly. This project integrates essential functionalities such as email verification, Google OAuth login, Stripe payment, Google Maps & Directions API, and SQL database with **Neon**.

---

## 🛠️ Features

- **User Authentication with Clerk**: Secure email login and email verification system with Clerk, ensuring users verify their accounts via email verification codes.
  
- **Google OAuth for Easy Login**: Users can log in quickly using their Google account, implemented via **Clerk** to streamline the OAuth process.

- **SQL Database with Neon Serverless**: **Neon** provides a highly scalable SQL database backend for seamless data management. Some advantages of using Neon:
  - **Serverless**: Neon offers a serverless experience, ensuring cost efficiency and scalability.
  - **High Availability**: It’s designed for modern applications, providing automatic scaling and availability.
  - **Developer-friendly**: Easy setup, management, and integration with PostgreSQL, making it suitable for large-scale applications.

- **Stripe Payment Integration**: Payments are securely handled using Stripe. The app runs in **test mode** for development safety, making it easy to test without processing real transactions.

- **Google Maps & Directions**: The app integrates **Google Maps** and **Google Directions API**, allowing users to see the route to their selected destinations. **React-Native-Maps-Directions** is used to render directions visually.

- **Driver and Ride Selection**: Users can search for locations and choose a driver based on availability. They get detailed information on ride cost, time to destination, and driver details before confirming.

- **Recent Rides Display**: Users can view their past rides on the home screen, providing a history of trips for easy access and review.

---

## 🧭 Workflow

1. **Login and Authentication**: 
   - Users can log in with their email or Google account using Clerk.
   - Email verification ensures that only verified users proceed further.

2. **Homepage with Map View**:
   - Once authenticated, the user is taken to a home screen displaying their current location on a map and a list of recent rides.
  
3. **Ride Booking**:
   - Users search for a location they want to go to, select a driver, and receive detailed information about the ride, including the fare, time to destination, and driver details.

4. **Stripe Payment**:
   - Once a ride is confirmed, users proceed with the payment using **Stripe** in test mode.
  
5. **Confirmation and Redirect**:
   - Upon successful payment, the user is redirected to the homepage, where the ride will be listed in the recent rides section.

---

## 🚀 Getting Started

### Prerequisites
To clone and run the app successfully, ensure you have the following API keys:

1. **Clerk API Key**: For email and Google OAuth authentication.
2. **Google Maps & Directions API Key**: To display and calculate routes in the app.
3. **Stripe API Key**: For handling payments in test mode.
4. **Neon Database Credentials**: To connect the app to the SQL database backend.

### Installation

1. Clone the repository:

   ```powershell
   git clone https://github.com/akachi11/Ryde.git
2. Navigate into the project directory:

    ```powershell
    cd Ryde
3. Install dependencies
   ```powershell
   npm install
4. Create a .env file and insert your api keys
   ```powershell
   EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=
   EXPO_PUBLIC_DATABASE_URL=
   EXPO_PUBLIC_SERVER_URL=
   EXPO_PUBLIC_GEOAPIFY_API_KEY=
   EXPO_PUBLIC_GOOGLE_API_KEY=
   EXPO_PUBLIC_STRIPE_PUBLISHABLE_KEY=
   STRIPE_SECRET_KEY=
5. Run the app
   ```powershell
   npm start


## 💡 Troubleshooting
The app has been built to handle several error cases, but you might encounter some issues during development or deployment. If you face any problems, don’t hesitate to reach out by opening an issue or contacting me via email.

## Feel free to reach out on my twitter if you have any questions or suggestions regarding the project! 😊

Made with ❤️ by Adika
