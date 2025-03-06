## Installation

To get started, install the required dependencies:

```bash
pip install psycopg2 dotenv
To install and configure PostgreSQL on Windows and Linux, follow these instructions:

### Windows

1. Download the PostgreSQL installer from the [official PostgreSQL website](https://www.postgresql.org/download/windows/).
2. Run the installer and follow the setup wizard steps.
3. During the installation, set a password for the PostgreSQL superuser (postgres).
4. After installation, open the SQL Shell (psql) and connect to your PostgreSQL server using the superuser credentials.

### Linux

1. Update your package lists:

```bash
sudo apt update
```

2. Install PostgreSQL:

```bash
sudo apt install postgresql postgresql-contrib
```

3. Start the PostgreSQL service:

```bash
sudo systemctl start postgresql
```

4. Enable PostgreSQL to start on boot:

```bash
sudo systemctl enable postgresql
```

5. Switch to the postgres user and open the PostgreSQL prompt:

```bash
sudo -i -u postgres
psql
```

6. Set a password for the postgres user:

```sql
\password postgres
```

For more detailed instructions, refer to the [official PostgreSQL documentation](https://www.postgresql.org/docs/).


## Configuration

1. Rename the `.example.env` file to `.env`.
2. Add your PostgreSQL variables to the `.env` file.

```env
DB_NAME=your_database_name
DB_USER=your_database_user
DB_PASSWORD=your_database_password
DB_HOST=your_database_host
DB_PORT=your_database_port
```

Make sure to replace the placeholder values with your actual PostgreSQL configuration.

