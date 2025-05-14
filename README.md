# Test
## Scenario

You are a Data Engineer for the new pet hotel Happy Whiskers. This hotel is a Romanian StartUp in animal care services and offers hotel services to its pet clients. 
## Business requirments
Happy Whiskers aims for a successful entry into the job market. The company provides hotel services for small to medium-sized domestic pets, as well as for exotic animals.

## Core Business Goals
1. *Get known on the market*
2. *Gaining and retaining clients by addressing their specific needs and expectations.*

## Reports
Buy cleaning products, care items, food supplies from manufacturers.\

#### KPIs
Average transaction amount.
Top 15 in Romanian buyers' preferences for pet hotel regimes


# Data Warehouse design
The hotel has a server InternIT anda database named `internit_db`.

### Sources
The company has the following data sources:
- InternIT - Own Platform Data
- [PetsGlobal](https://www.petsglobal.com/) - Partner Platform for animal product supplies.

#### InternIT Source
`internit_data`

| Column Name | Data Type | Description |
| ----- | ----- | ----- |
| booking_id | VARCHAR(50) | Unique idendifier for the booking |
| pet_name | VARCHAR(50) | Pet name |
| owner_first_name | VARCHAR(50) | Owner first name |
| owner_last_name | VARCHAR(50) | Owner last name |
| pet_id | VARCHAR(50) | Unique identifier for the pet |
| pet_species | VARHAR(255) | The species of the pet |
| pet_size | VARCAHR(100) | The size of the pet |
| check_in | TIMESTAMP | The time of the check_in |
| check_out | TIMESTAMP | The time of the check_out |
| amount | INT | Amount of money of the transactin |
| type | VARCHAR(15) | Type of the transaction |
| time | TIMESTAMP | Transaction time |


`PetsGlobal`
| Column Name | Data Type | Description |
| ----- | ----- | ----- |
| product_type | VARCHAR(255) | Type of the supply\product |
| product_amount | INT | Amont of the supply\product |
| manufacturer | VARCHAR(255) | Manufacturer of the supply\product



