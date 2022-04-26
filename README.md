# ENSF-614 Term Project

A project on Movie Theater Ticket Reservation App. Please refer to the [project description document](docs/Project_Description.pdf) for more information.

## Project Structure

![dir tree](images/structure.png)

- [`config`](config) - contains the config files containing important settings for the project to work

- [`docs`](docs) - various documents, including system diagrams, of the project

  - [`docs/javadoc.zip`](docs/javadoc.zip) - javadoc as zip archive

- [`lib`](lib) - contains the JARs used by the project

- [`src`](src) - contains all the source code as `.java` files

## How to run

1. Clone the repository to your local machine.

2. Start the MySQL server on your local machine.

3. Open the file [config/db_details.properties](config/db_details.properties) and enter your Db server details. For `db.user` and `db.password`, enter your DB user login details. Please use a user that has all the CRUD access, like `root`.

4. Connect to your MySQL server using an user used in step 3.

5. Run [this](ENSF614_Project_Database.sql) script on the MySQL server. This script will create a schema **ENSF614PROJECT**, create all necessary tables, and load them with some dummy data.

6. To compile the source code, run the below command

   ```bash
   $ javac -cp ".;lib/*" -sourcepath "src" -d "bin" src/movieTicketSystem/*java src/movieTicketSystem/controller/*java src/movieTicketSystem/model/*java src/movieTicketSystem/view/*java
   ```

7. To run the source code, run the below command
   ```bash
   $ java -cp ".;lib/*;bin" movieTicketSystem.movieApp
   ```

## Contributors

- [Giese, Calvin](https://github.com/calvingiese)
- [Guo, Yuhua](https://github.com/davedaveisguo)
- [Gupta, Bhavyai](https://github.com/zbhavyai)
- [Hall, Graydon ](https://github.com/GraydonHall42)
