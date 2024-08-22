# Supplier-Details API for MakerSharks

This project provides an API to manage and search for supplier details as part of a proof of concept for MakerSharks.

## Requirements

- **Java Version**: 21
- **MySQL Server**: 8.0
- **IDE**: IntelliJ IDEA / Eclipse / Spring Suite Tool / NetBeans / VSCode
- **API Testing Tool**: Postman

## Setup Instructions

### 1. Project Import

- Import the project as a Maven project into your preferred IDE.

### 2. Database Configuration

- Create a MySQL database named `supplier_details`.
- Update the `application.properties` file with your MySQL configuration:
  ```properties
  spring.datasource.url=jdbc:mysql://localhost:3306/supplier_details
  spring.datasource.username=YOUR_MYSQL_USERNAME
  spring.datasource.password=YOUR_MYSQL_PASSWORD
- Replace YOUR_MYSQL_USERNAME and YOUR_MYSQL_PASSWORD with your MySQL credentials.
###  3. Running the Application

  -  Run the MakerSharksApplication.java file from your IDE to start the application.

# Important Notes
### Data Format Requirements
   - Ensure that the natureOfBusiness field in your JSON requests is in UPPERCASE with one of the following values: SMALL_SCALE, MEDIUM_SCALE, or LARGE_SCALE.
   - The manufacturingProcesses field must also be in UPPERCASE and can take one of the following values: MOULDING, THREE_D_PRINTING, CASTING, COATING.

## Sample JSON Data

Here is a sample JSON array for testing purposes:
```

[
    {
        "supplierId": 1,
        "companyName": "ABC Manufacturing",
        "website": "http://www.abcmfg.com",
        "location": "New York",
        "natureOfBusiness": "SMALL_SCALE",
        "manufacturingProcesses": "MOULDING"
    },
    {
        "supplierId": 2,
        "companyName": "XYZ Industries",
        "website": "http://www.xyzindustries.com",
        "location": "Los Angeles",
        "natureOfBusiness": "MEDIUM_SCALE",
        "manufacturingProcesses": "THREE_D_PRINTING"
    },
    {
        "supplierId": 3,
        "companyName": "Global Casting Co.",
        "website": "http://www.globalcasting.com",
        "location": "Chicago",
        "natureOfBusiness": "LARGE_SCALE",
        "manufacturingProcesses": "CASTING"
    },
    {
        "supplierId": 4,
        "companyName": "Precision Coating Ltd.",
        "website": "http://www.precisioncoating.com",
        "location": "San Francisco",
        "natureOfBusiness": "SMALL_SCALE",
        "manufacturingProcesses": "COATING"
    },
    {
        "supplierId": 5,
        "companyName": "Tech Innovations",
        "website": "http://www.techinnovations.com",
        "location": "Austin",
        "natureOfBusiness": "MEDIUM_SCALE",
        "manufacturingProcesses": "THREE_D_PRINTING"
    }
]
