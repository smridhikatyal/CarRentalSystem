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

Installation
Clone the repository:

git clone https://github.com/smridhikatyal/car-rental-system.git
Navigate to the project directory:

cd car-rental-system
Compile the Java files:

javac car_rental_system/*.java
Run the application:

java car_rental_system.Main

Usage
Once the application is running, follow the on-screen prompts to:

Car Rental System
This is a simple Car Rental System implemented in Java using Object-Oriented Programming (OOP) principles. The system allows customers to rent and return cars. The system tracks available cars, customers, and rental transactions.

Features
Add cars to the rental system
Add customers to the system
Rent available cars to customers
Return rented cars
Calculate the total price for a rental period
Classes
Car
Represents a car in the rental system.

Attributes:

String carId
String brand
String model
double basePricePerDay
boolean isAvailable
Methods:

Car(String carId, String brand, String model, double basePricePerDay)
String getCarId()
String getBrand()
String getModel()
double calculatePrice(int rentalDays)
boolean isAvailable()
void rent()
void returnCar()
Customer
Represents a customer in the rental system.

Attributes:

String customerId
String name
Methods:

Customer(String customerId, String name)
String getCustomerId()
String getName()
Rental
Represents a rental transaction.

Attributes:

Car car
Customer customer
int days
Methods:

Rental(Car car, Customer customer, int days)
Car getCar()
Customer getCustomer()
int getDays()
CarRentalSystem
The main system class that manages cars, customers, and rentals.

Attributes:

List<Car> cars
List<Customer> customers
List<Rental> rentals
Methods:

CarRentalSystem()
void addCar(Car car)
void addCustomer(Customer customer)
void rentCar(Car car, Customer customer, int days)
void returnCar(Car car)
void menu()
Usage
Add Cars: Initialize the CarRentalSystem and add cars to it.
Add Customers: Customers are added when they rent a car.
Rent a Car: Customers can rent a car if it is available.
Return a Car: Customers can return rented cars.
Menu: The system provides a menu for renting and returning cars.
