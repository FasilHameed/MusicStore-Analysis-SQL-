# SQL Project: Music Store Analysis

## Database Schema: Music Store Database

### Tables

#### 1. Customers
- **customer_id** (Primary Key): Unique identifier for each customer
- first_name: First name of the customer
- last_name: Last name of the customer
- email: Email address of the customer
- phone: Phone number of the customer
- address: Address of the customer
- city: City where the customer resides
- state: State where the customer resides
- country: Country where the customer resides
- postal_code: Postal code of the customer's address

#### 2. Employees
- **employee_id** (Primary Key): Unique identifier for each employee
- last_name: Last name of the employee
- first_name: First name of the employee
- birth_date: Birth date of the employee
- hire_date: Hire date of the employee
- address: Address of the employee
- city: City where the employee resides
- state: State where the employee resides
- country: Country where the employee resides
- postal_code: Postal code of the employee's address
- phone: Phone number of the employee
- email: Email address of the employee

#### 3. Invoices
- **invoice_id** (Primary Key): Unique identifier for each invoice
- customer_id (Foreign Key): Corresponds to the customer who made the purchase
- invoice_date: Date when the invoice was issued
- billing_address: Billing address for the invoice
- billing_city: City for the billing address
- billing_state: State for the billing address
- billing_country: Country for the billing address
- billing_postal_code: Postal code for the billing address
- total: Total amount of the invoice

#### 4. Invoice_Items
- **invoice_line_id** (Primary Key): Unique identifier for each invoice line item
- invoice_id (Foreign Key): Corresponds to the invoice to which the item belongs
- track_id (Foreign Key): Corresponds to the purchased track
- unit_price: Price per unit of the track
- quantity: Quantity of the track purchased

#### 5. Tracks
- **track_id** (Primary Key): Unique identifier for each track
- name: Name of the track
- album_id (Foreign Key): Corresponds to the album to which the track belongs
- media_type_id (Foreign Key): Corresponds to the media type of the track
- genre_id (Foreign Key): Corresponds to the genre of the track
- composer: Composer of the track
- milliseconds: Duration of the track in milliseconds
- bytes: Size of the track file in bytes
- unit_price: Price per unit of the track

#### 6. Albums
- **album_id** (Primary Key): Unique identifier for each album
- title: Title of the album
- artist_id (Foreign Key): Corresponds to the artist of the album

#### 7. Artists
- **artist_id** (Primary Key): Unique identifier for each artist
- name: Name of the artist

#### 8. Genres
- **genre_id** (Primary Key): Unique identifier for each genre
- name: Name of the genre

#### 9. Media_Types
- **media_type_id** (Primary Key): Unique identifier for each media type
- name: Name of the media type

## Database Management System and Tools

- **DBMS Used:** PostgreSQL
- **Database Client:** PgAdmin4

## Database Schema Visualization

![MusicDatabaseSchema](https://user-images.githubusercontent.com/112153548/213707717-bfc9f479-52d9-407b-99e1-e94db7ae10a3.png)

## Repository Link

[GitHub Repository](https://github.com/FasilHameed/MusicStore-Analysis-SQL-.git)
