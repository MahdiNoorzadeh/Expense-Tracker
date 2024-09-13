# Trustly Wallet

Trustly Wallet is a simple and user-friendly application that helps you track your expenses over time. The app allows you to monitor your daily transactions and gives an overview of your income and expenses for better financial planning.

## Features

- **Expense Tracking:** The app automatically tracks your expenses for the last seven days.
- **Customizable Time Period:** You can easily adjust the default tracking period by editing the source code.
- **User-Friendly Interface:** Intuitive and easy-to-use interface to manage your financial data.

## Requirements

- .NET 6.0 or later
- SQL Server

## Installation

### 1. Clone the Repository
Clone this project to your local machine using Git:
```bash
git clone https://github.com/yourusername/trustly-wallet.git
```
### 2. Database Configuration
You'll need to configure the connection to your SQL Server database.
Open appsettings.json.
Update the ConnectionStrings section with your own database credentials:
```
"ConnectionStrings": {
   "DevConnection": "Server=YOUR_SERVER;Database=YOUR_DATABASE;Trusted_Connection=True;MultipleActiveResultSets=True;TrustServerCertificate=True;"
}
```
### 3. Customizing the Expense Tracking Period
By default, the app tracks expenses for the last seven days. If you'd like to change this:
Navigate to the Controllers/DashboardController.cs.
Find the line with the comment // Combining Income and expenses.
Change the logic to fit your desired time range.

Thanks to https://www.youtube.com/@CodAffection for the tutorial. Here is the link to the tutorial on the project: https://youtu.be/zQ5eijfpuu8

### Happy Coding!. 
