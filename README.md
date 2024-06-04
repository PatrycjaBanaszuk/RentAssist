# RentAssist
RentAssist is a Java application that helps social housing organizations manage rent collection and prevent rent arrears. 
It uses predictive analytics to find tenants who might miss payments and sends alerts to take action.


## Features

- **Predictive Analytics**: Uses data to predict which tenants are likely to fall into arrears.
- **Real-Time Monitoring**: Keeps track of rent payments in real-time.
- **Alerts and Notifications**: Sends alerts for overdue payments and potential risks.
- **Tenant Management**: Maintains detailed records of tenant payment histories.
- **Reporting Tools**: Generates reports to help housing organizations make informed decisions.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Java Development Kit (JDK) 8 or higher
- Apache Maven
- MySQL or another relational database

### Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/PatrycjaBanaszuk/RentAssist.git
    ```
2. **Navigate to the project directory**:
    ```bash
    cd RentAssist
    ```
3. **Install dependencies**:
    ```bash
    mvn clean install
    ```
4. **Set up the database**:
    - Create a MySQL database named `rentassist`.
    - Update the database configuration in `src/main/resources/application.properties`.

    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/rentassist
    spring.datasource.username=root
    spring.datasource.password=yourpassword
    ```

5. **Run the application**:
    ```bash
    mvn spring-boot:run
    ```

## Usage

Once the application is running, you can access it at `http://localhost:8080`. The following endpoints are available:

- `GET /tenants` - Retrieve a list of all tenants.
- `POST /tenants` - Add a new tenant.
- `GET /tenants/{id}` - Retrieve details of a specific tenant.
- `PUT /tenants/{id}` - Update a tenant's information.
- `DELETE /tenants/{id}` - Delete a tenant.

## Built With

- [Spring Boot](https://spring.io/projects/spring-boot) - Framework for building Java applications
- [Hibernate](https://hibernate.org/) - ORM tool for database interactions
- [MySQL](https://www.mysql.com/) - Relational database management system


## Authors

- **Your Name** - *Initial work* - [Patrycja Banaszuk](https://github.com/PatrycjaBanaszuk)


