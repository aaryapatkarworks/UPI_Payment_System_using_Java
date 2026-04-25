# Smart UPI System

A comprehensive Java-based UPI (Unified Payments Interface) payment system with a modern graphical user interface built using JavaFX.

## Features

### Core Functionality
- **User Registration & Login**: Secure user authentication with PIN validation
- **Send Money**: Transfer funds to other UPI IDs with PIN verification
- **Receive Money**: Generate QR codes and payment request links
- **Transaction History**: View detailed transaction records with filtering options
- **Dashboard**: Real-time balance display and quick access to all features

### Advanced Features
- **QR Code Generation**: Visual QR codes for easy payments
- **Payment Requests**: Generate shareable payment links
- **Transaction Filtering**: Filter by type, date, and amount
- **Security Features**: PIN-based authentication and validation
- **Modern UI**: Clean, intuitive interface with color-coded transactions

## Technology Stack

- **Java 11**: Core programming language
- **JavaFX 17**: Modern GUI framework
- **Maven**: Build and dependency management
- **ZXing**: QR code generation
- **Jackson**: JSON processing
- **JUnit 5**: Unit testing

## Project Structure

```
src/main/java/com/upi/
├── Main.java                    # Application entry point
├── Dashboard.java               # Main dashboard screen
├── RegistrationScreen.java     # User registration
├── SendMoneyScreen.java         # Send money interface
├── ReceiveMoneyScreen.java      # Receive money interface
└── TransactionHistory.java     # Transaction history viewer
```

## Installation & Setup

### Prerequisites
- Java Development Kit (JDK) 11 or higher
- Maven 3.6 or higher
- IDE with JavaFX support (IntelliJ IDEA, Eclipse, or VS Code)

### Building the Project

1. Clone or download the project
2. Navigate to the project directory
3. Run the following commands:

```bash
# Compile the project
mvn clean compile

# Run the application
mvn javafx:run

# Create executable JAR
mvn clean package
```

### Running the Application

**Method 1: Using Maven**
```bash
mvn javafx:run
```

**Method 2: Using the executable JAR**
```bash
java -jar target/smart-upi-system-1.0-SNAPSHOT.jar
```

**Method 3: Running from IDE**
- Run the `Main.java` class directly from your IDE

## Usage Guide

### 1. Registration
- Click "Register" on the login screen
- Fill in your personal details
- Create a 4-digit PIN
- Select your bank from the dropdown

### 2. Login
- Enter your UPI ID (format: name@upi)
- Enter your 4-digit PIN
- Click "Sign In"

### 3. Dashboard Features
- **Balance Display**: View your available balance
- **Quick Actions**: Access Send, Receive, QR Scan, and History
- **Recent Transactions**: See your latest transactions

### 4. Sending Money
- Enter recipient's UPI ID
- Enter the amount
- Add an optional remark
- Confirm with your PIN

### 5. Receiving Money
- View your QR code for scanning
- Generate payment request links
- Share your UPI ID with others

### 6. Transaction History
- View all past transactions
- Filter by type (Sent/Received/Failed)
- Filter by time period
- See transaction summaries

## Demo Data

For demonstration purposes, the application includes:
- Default balance: ₹10,000.00
- Sample transaction history
- Mock bank selection options

## Future Enhancements

### Planned Features
- [ ] Real database integration (MySQL/PostgreSQL)
- [ ] Actual QR code scanning with camera
- [ ] Biometric authentication
- [ ] Multi-language support
- [ ] Export transaction statements
- [ ] Payment scheduling
- [ ] Split bills feature
- [ ] Integration with real banking APIs

### Security Improvements
- [ ] End-to-end encryption
- [ ] Two-factor authentication
- [ ] Session management
- [ ] Audit logging

## Contributing

This project is developed as part of the Mini Project in Java (MPJ) course. 

## License

This project is for educational purposes only.

## Support

For any questions or issues, please contact the development team.

---

**Note**: This is a demonstration project and does not connect to real banking systems. All transactions are simulated for educational purposes.
