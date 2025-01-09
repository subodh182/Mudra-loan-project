# Mudra-loan-project
The MUDRA loans are provided for income generating small business activity in manufacturing, processing, service sector or trading. The Project cost is decided based on business plan and the investment proposed. MUDRA loan is not for consumption/personal needs.
# Mudra Loans Project

## Overview
The **Mudra Loans Project** is designed to streamline and simplify the process of availing loans under the Pradhan Mantri Mudra Yojana (PMMY). This system provides an easy-to-use platform for individuals and small businesses to apply for loans, track their applications, and gain insights into loan eligibility criteria.

## Installation

### Prerequisites
- Node.js and npm
- MongoDB instance (local or cloud-based)
- Git installed

### Steps
1. **Clone the repository**:
    ```bash
    git clone https:/https://github.com/subodh182/Mudra-loan-project/github.com//mudra-loans.git
    cd mudra-loans
    ```

2. **Install dependencies**:
    ```bash
    npm install
    cd client && npm install
    ```

3. **Set up environment variables**:
    Create a `.env` file in the root directory and add:
    ```env
    PORT=5000
    MONGO_URI=your-mongodb-uri
    JWT_SECRET=your-secret-key
    CLIENT_URL=http://localhost:3000
    ```

4. **Run the application**:
    - Start the backend server:
      ```bash
      npm run dev
      ```
    - Start the frontend:
      ```bash
      cd client
      npm start
      ```

5. **Access the application**:
   Open `http://localhost:3000` in your web browser.

## Project Structure
```
|-- mudra-loans
    |-- client            # Frontend files
    |   |-- public
    |   |-- src
    |-- server            # Backend files
        |-- models        # Mongoose schemas
        |-- routes        # API routes
        |-- controllers   # Request handlers
        |-- utils         # Utility functions
    |-- .env.example      # Example environment variables
    |-- package.json      # Backend dependencies
    |-- README.md         # Project documentation
```

## API Endpoints

### User Endpoints
- **POST** `/api/users/register`: Register a new user.
- **POST** `/api/users/login`: Authenticate a user.

### Loan Endpoints
- **POST** `/api/loans/apply`: Submit a loan application.
- **GET** `/api/loans/status/:id`: Check loan application status.

### Admin Endpoints
- **GET** `/api/admin/applications`: View all loan applications.
- **POST** `/api/admin/update-status`: Update loan status.

## Contribution Guidelines
1. Fork the repository.
2. Create a new branch for your feature/bug fix:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature description"
   ```
4. Push your changes:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgments
- Pradhan Mantri Mudra Yojana (PMMY) guidelines.
- Open-source libraries and contributors.
