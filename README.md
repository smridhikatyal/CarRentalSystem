# CarRentalSystem


 Car Rental System
This project implements a simple car rental system using Java. The system allows customers to rent and return cars, providing a basic interface for these operations.

Table of Contents
Features
Installation
Usage
Classes and Methods
Example
License
Features
Add cars to the system.
Add customers to the system.
Rent available cars to customers.
Return rented cars.
Calculate rental price based on the number of days.
Basic console-based user interface.
Installation
Clone the repository:

git clone https://github.com/your-username/car-rental-system.git
Navigate to the project directory:

cd car-rental-system
Compile the Java files:

javac car_rental_system/*.java
Run the application:

java car_rental_system.Main

Usage
Once the application is running, follow the on-screen prompts to:

Rent a car: Enter your name, choose an available car by its ID, and specify the number of rental days.
Return a car: Enter the car ID you want to return.
Classes and Methods
Car
Represents a car in the rental system.

Car(String carId, String brand, String model, double basePricePerDay): Constructor to initialize a car.
String getCarId(): Returns the car ID.
String getBrand(): Returns the car brand.
String getModel(): Returns the car model.
double calculatePrice(int rentalDays): Calculates the rental price for the specified number of days.
boolean isAvailable(): Checks if the car is available for rent.
void rent(): Marks the car as rented.
void returnCar(): Marks the car as available.
Customer
Represents a customer in the rental system.

Customer(String customerId, String name): Constructor to initialize a customer.
String getCustomerId(): Returns the customer ID.
String getName(): Returns the customer name.
Rental
Represents a rental transaction.

Rental(Car car, Customer customer, int days): Constructor to initialize a rental.
Car getCar(): Returns the rented car.
Customer getCustomer(): Returns the customer who rented the car.
int getDays(): Returns the number of rental days.
CarRentalSystem
Manages the car rental system.

CarRentalSystem(): Constructor to initialize the car rental system.
void addCar(Car car): Adds a car to the system.
void addCustomer(Customer customer): Adds a customer to the system.
void rentCar(Car car, Customer customer, int days): Rents a car to a customer for the specified number of days.
void returnCar(Car car): Returns a rented car.
void menu(): Displays the main menu and handles user input.
