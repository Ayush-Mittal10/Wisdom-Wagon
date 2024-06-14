# Wisdom Wagon

Wisdom Wagon is an online platform offering a wide range of coding courses and resources to help learners enhance their coding skills. It provides courses in various domains such as Web Development, Programming, Data Science, and more.

![Wisdom Wagon Screenshot](./demo/screenshot.png)

## Features

- **Wide Range of Courses**: Choose from a variety of courses tailored to different skill levels and interests.
- **Course Details**: Each course page includes comprehensive details such as instructor information, course description, skills gained, and student reviews.
- **User Authentication**: Secure user authentication system for logging in and signing up.
- **Shopping Cart**: Integrated shopping cart feature to add courses for future purchase.
- **Payment Integration**: Seamless payment integration using Razorpay for purchasing courses.
- **Responsive Design**: Fully responsive design for a seamless experience across devices.

## Technologies Used

- **Frontend**: React.js, React Router, HTML5, CSS3, JavaScript
- **Backend**: Node.js, Express.js, MongoDB
- **Payment Gateway**: Razorpay
- **Others**: JWT (JSON Web Tokens), Multer (for file uploads), Axios (for API requests)

## Getting Started

### Prerequisites

- Node.js installed on your local environment
- MongoDB installed and running locally or accessible via MongoDB Atlas

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/wisdom-wagon.git
   cd wisdom-wagon
   ```

2. Install dependencies for both frontend and backend:

   ```bash
   # Install backend dependencies
   cd backend
   npm install

   # Install frontend dependencies
   cd ../frontend
   npm install
   ```

### Configuration

1. Backend Configuration:

   - Create a `.env` file in the `backend` directory and add the following environment variables:

     ```
     DATABASE=mongodb://localhost:27017/wisdom-wagon
     RAZORPAY_KEY_ID=<Your_Razorpay_Key_ID>
     RAZORPAY_SECRET=<Your_Razorpay_Secret>
     ```

2. Frontend Configuration:

   - Update the Razorpay configuration in `CoursePage.js` with your Razorpay key details:

     ```javascript
     let options = {
       key: "<Your_Razorpay_Key_ID>",
       // Other Razorpay options
     };
     ```

### Running the Application

1. Start the backend server:

   ```bash
   cd backend
   npm start
   ```

   The server should start on `http://localhost:3000`.

2. Start the frontend development server:

   ```bash
   cd frontend
   npm start
   ```

   The frontend should open automatically in your default browser at `http://localhost:3001`.

### Usage

- Browse courses, view details, add them to the cart, and proceed to checkout.
- Explore different categories and search for courses by name.
- Login or signup to manage your profile and access purchased courses.

### Contributing

Contributions are welcome! Here's how you can contribute to Wisdom Wagon:

1. Fork the repository and create your branch: `git checkout -b feature/my-feature`.
2. Commit your changes: `git commit -am 'Add new feature'`.
3. Push to the branch: `git push origin feature/my-feature`.
4. Submit a pull request.

### License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

### Acknowledgements

- **Icons**: Ionicons
- **Images**: Unsplash
