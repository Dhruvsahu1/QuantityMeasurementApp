# Quantity Measurement App
 
> Project — Unit conversion application supporting multiple physical quantity types with a clean N-Tier architecture.
 
---
 
## Table of Contents
 
1. [Overview](#overview)
2. [Supported Units](#supported-units)
3. [Folder Structure](#folder-structure)
4. [Use Cases](#use-cases)
5. [Important Information](#important-information)
 
---
 
## Overview
 
The **Quantity Measurement App** is designed to facilitate the conversion and measurement of various physical quantities. It supports multiple measurement units and provides a structured, easy-to-use interface suitable for users of all technical backgrounds.
 
This project was developed as part of the **Capgemini Java Training Program**, focusing on object-oriented design principles, test-driven development (TDD), and a clean N-Tier layered architecture.
 
**Key Highlights:**
 
- Accurate unit conversion across multiple quantity families
- Type-safe implementation using `Double.compare()` and null checks
- JUnit 5 test coverage for all 15 use cases
- Refactored into N-Tier Architecture (UC15)
 
---
 
## Supported Units
 
| Category    | Units Supported                               |
|-------------|-----------------------------------------------|
| Length      | Meters, Kilometers, Miles, Yards, Feet, Inches |
| Weight      | Grams, Kilograms, Pounds, Ounces              |
| Temperature | Celsius, Fahrenheit, Kelvin                   |
| Volume      | Litre, MilliLitre, Gallon                     |
 
---
 
## Folder Structure
 
```
quantity-measurement-app/
├── src/
│   ├── main/
│   │   └── java/com/qma/
│   │       ├── model/          # Domain entities (Length, Weight, Temperature, Volume)
│   │       ├── service/        # Business logic and conversion operations
│   │       ├── repository/     # Data access layer
│   │       └── controller/     # Application entry points
│   └── test/
│       └── java/com/qma/
│           ├── LengthTest.java
│           ├── TemperatureTest.java
│           ├── VolumeTest.java
│           └── WeightTest.java
├── pom.xml
└── README.md
```
 
---
 
## Use Cases
 
The application is validated through 15 use cases, each covering a specific conversion scenario or design concern.
 
| Use Case | Title                              | Key Concepts                                      |
|----------|------------------------------------|---------------------------------------------------|
| UC-01    | Feet Measurement Equality          | `Double.compare()`, null checking, type safety    |
| UC-02    | Feet to Inches Conversion          | Unit conversion logic, conversion factors         |
| UC-03    | Inch Measurement                   | Symmetrical class design                          |
| UC-04    | Feet and Inch Addition             | Unit standardization, arithmetic operations       |
| UC-05    | Yard Measurement                   | Multi-level unit hierarchy                        |
| UC-06    | Centimeter Measurement             | Metric system introduction                        |
| UC-07    | Centimeter to Meter Conversion     | Metric hierarchy                                  |
| UC-08    | Imperial to Metric Conversion      | Cross-family conversions                          |
| UC-09    | Kilometer Distance Measurement     | Extended metric system                            |
| UC-10    | Mile Measurement                   | Imperial long-distance units                      |
| UC-11    | Temperature Conversion             | Non-linear transformations (offset arithmetic)    |
| UC-12    | Volume Measurement                 | Litres and Millilitres                            |
| UC-13    | Weight Measurement                 | Grams and Kilograms                               |
| UC-14    | Compound Conversion and Addition   | Multi-dimensional unit handling                   |
| UC-15    | Refactor into N-Tier Architecture  | Layered architecture, separation of concerns      |
 
---
 
## Important Information
 
- Ensure the required permissions are configured in your environment before running the application.
- Temperature conversions involve non-linear formulas. Always use `Double.compare()` for floating-point equality checks — avoid using `==`.
- All use cases are backed by JUnit 5 test suites. Run `mvn test` to execute the full suite before deployment.
- Follow the guidelines in the user manual for best results and consistent behaviour across unit families.
 
---
  
> **Technology Stack:** Java · JUnit 5 · Maven · N-Tier Architecture
