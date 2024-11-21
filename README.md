# POE

# Contract Monthly Claim System (CMCS)

The **Contract Monthly Claim System (CMCS)** is a web-based application designed to streamline the process of submitting, tracking, and managing monthly claims for contracts. This system allows users to submit claims, view submitted claims, and receive confirmation for key actions like registration and login. It aims to simplify contract management for users and improve efficiency within the organization.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Database Setup](#database-setup)
- [Usage](#usage)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)

## Features
- **User Registration and Login**: Secure authentication for new and returning users with feedback messages after successful registration or login.
- **Claim Submission**: Users can submit monthly claims, which are stored and tracked within the system.
- **View Submitted Claims**: Users can view a list of all previously submitted claims for reference and auditing.
- **Confirmation and Feedback**: Confirmation messages are provided after submitting forms, enhancing user experience.

## Technologies Used
- **ASP.NET Core** - Backend framework for creating web APIs and services
- **Entity Framework Core** - ORM for database operations
- **SQL Database** - Database management
- **HTML/CSS** - Frontend design
- **JavaScript** - Enhancing user interactivity

## Getting Started
Follow these steps to set up and run the project locally.

### Prerequisites
- [.NET Core SDK](https://dotnet.microsoft.com/download)
- SQL Server or any other compatible database

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/contract-monthly-claim-system.git
   ```
2. Navigate to the project directory:
   ```bash
   cd contract-monthly-claim-system
   ```
3. Install the required packages:
   ```bash
   dotnet restore
   ```

## Database Setup
1. Configure your database connection in `appsettings.json`:
   ```json
   "ConnectionStrings": {
     "DefaultConnection": "YourConnectionStringHere"
   }
   ```
2. Run database migrations:
   ```bash
   dotnet ef database update
   ```
3. If necessary, ensure you have the following packages installed:
   ```bash
   dotnet add package Microsoft.EntityFrameworkCore.SqlServer
   dotnet add package Microsoft.EntityFrameworkCore.Tools
   ```

## Usage
1. Start the application:
   ```bash
   dotnet run
   ```
2. Open your browser and navigate to `https://localhost:5001` (or the port shown in the console).

### Key Pages
- **Register and Login Pages**: Create a new account or log in to an existing account.
- **Submit Claims**: Users can fill out and submit their monthly contract claims here.
- **View Submitted Claims**: Access a list of all claims previously submitted.

## Future Improvements
- **Notifications**: Integrate email or in-app notifications for submission status updates.
- **Admin Dashboard**: Add an administrative dashboard for tracking and managing all user claims.
- **Reporting**: Implement reporting features for generating claim summaries and analysis.

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License
This project is licensed under the MIT License.
