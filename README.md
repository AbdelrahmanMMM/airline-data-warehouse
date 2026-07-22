# ✈️ Enterprise Airline Data Warehouse

> Enterprise Data Warehouse implementation for an airline reservation system using **IBM DataStage**, **Oracle Database**, and **Kimball Dimensional Modeling**.

![Architecture](images/dimensional_model.png)

---

## 📖 Overview

This project demonstrates the end-to-end development of an enterprise Data Warehouse for an airline company using the Kimball methodology.

The warehouse integrates data from Oracle databases and CSV files into a centralized analytical repository through ETL pipelines developed in IBM DataStage.

The project covers dimensional modeling, surrogate key generation, star schema design, ETL development, data validation, and loading of multiple fact and dimension tables.

---

## 🚀 Technologies

- IBM InfoSphere DataStage
- Oracle Database
- Oracle SQL
- PL/SQL
- Kimball Dimensional Modeling
- Star Schema
- ETL Development

---

# 🏗️ Data Warehouse Architecture

The warehouse follows the Kimball dimensional modeling approach.

- Dimension Tables
- Fact Tables
- Shared Date Dimension
- Surrogate Keys
- Star Schema Relationships

Insert the dimensional model here.

```text
images/
    dimensional_model.png
```

```markdown
![Dimensional Model](images/dimensional_model.png)
```

---

# 📊 Data Sources

The warehouse integrates data from multiple operational sources.

### Oracle Tables

- Airports
- Aircraft
- Routes
- Flights
- Fare Classes
- Booking Channels
- Frequent Flyer Tiers
- Passengers
- Reservations
- Tickets
- Payments

### CSV Files

- Promotions
- Promotion Responses
- Loyalty Miles Transactions
- Customer Interactions
- Flight Upgrades
- Overnight Stays

---

# ⭐ Star Schema

## Dimension Tables

- DIM_DATE
- DIM_PASSENGER
- DIM_AIRPORT
- DIM_ROUTE
- DIM_FLIGHT
- DIM_AIRCRAFT
- DIM_BOOKING_CHANNEL
- DIM_FARE_CLASS
- DIM_PROMOTION

---

## Fact Tables

- FACT_RESERVATION
- FACT_TICKET
- FACT_PAYMENT
- FACT_PROMOTION_RESPONSE
- FACT_LOYALTY_TRANSACTION
- FACT_CUSTOMER_INTERACTION
- FACT_UPGRADE
- FACT_OVERNIGHT_STAY

---

# 🔄 ETL Workflow

The ETL pipelines were implemented using IBM DataStage.

Each pipeline follows the standard ETL process:

Source

↓

Extract

↓

Transform

↓

Lookup Dimensions

↓

Generate Surrogate Keys

↓

Load Fact/Dimension Tables

↓

Validation

---

# ⚙️ ETL Features

✔ Oracle Connector

✔ Sequential File Stage

✔ Transformer Stage

✔ Join Stage

✔ Lookup Stage

✔ Key Generator

✔ Shared Date Dimension

✔ Surrogate Key Generation

✔ Data Validation

✔ Row Reconciliation

---

# 📂 Repository Structure

```
Enterprise-Airline-Data-Warehouse
│
├── README.md
│
├── images
│   ├── dimensional_model.png
│   ├── fact_reservation_job.png
│   ├── fact_payment_job.png
│   ├── dim_passenger_job.png
│   └── customer_interaction_job.png
│
├── sql
│   ├── create_dimensions.sql
│   ├── create_facts.sql
│   ├── create_date_dimension.sql
│   ├── validation_queries.sql
│   └── sample_queries.sql
│
├── datastage
│   ├── DIM_PASSENGER.dsx
│   ├── DIM_AIRPORT.dsx
│   ├── FACT_RESERVATION.dsx
│   ├── FACT_PAYMENT.dsx
│   ├── FACT_TICKET.dsx
│   └── ...
│
└── sample-data
    └── sample_csv_files
```

---

# 📸 Sample ETL Jobs

Example DataStage jobs included in this repository:

- Passenger Dimension
- Reservation Fact
- Payment Fact
- Customer Interaction Fact

Example screenshot:

```markdown
![FACT_RESERVATION](images/fact_reservation_job.png)
```

---

# 🗄️ SQL Scripts

The repository includes Oracle SQL scripts for:

- Warehouse creation
- Dimension tables
- Fact tables
- Date dimension
- Validation queries
- Testing queries

---

# ✅ Data Quality

During development the following validation checks were performed:

- Source vs Target row count reconciliation
- Surrogate key validation
- Dimension lookup verification
- Referential integrity validation
- Null value handling
- CSV parsing validation

---

# 💡 Skills Demonstrated

- Data Warehousing
- Kimball Methodology
- Star Schema Design
- IBM DataStage
- Oracle SQL
- PL/SQL
- ETL Development
- Data Integration
- Surrogate Keys
- Dimension Lookups
- Data Validation
- Oracle Database

---

# 📈 Learning Outcomes

This project provided practical experience in:

- Designing enterprise dimensional models
- Building ETL pipelines in IBM DataStage
- Loading dimensions and fact tables
- Integrating multiple heterogeneous data sources
- Implementing surrogate key generation
- Validating data quality throughout the ETL process

---

# 👤 Author

**Abdelrahman Malek Genedy**

Data Engineer

- LinkedIn: https://linkedin.com/in/abdelrahman-malek-genedy
- GitHub: https://github.com/AbdelrahmanMMM

---

## ⭐ If you found this project interesting, feel free to star the repository.
