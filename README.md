# 2201CS11_CS260

## Authors :

- Akhand Singh (2201CS11) [@akhandsinghjr](https://github.com/akhandsinghjr)
- Anchal Dubey (2201CS15) [@anchaldubey](https://github.com/anchaldubey)

## Youtube Link : https://youtu.be/TpbHbeYuWuI

## ER Diagrams :
- https://drive.google.com/file/d/1Z-sBhnY-cfMBXLjqaUVxxj0K003z61v4/view?usp=sharing 
- Also we have kept the pdf in the proj1 folder

## Used Technologies :
 
- <img src="https://static-00.iconduck.com/assets.00/node-js-icon-1817x2048-g8tzf91e.png" width="25" height="25"/>   NODE JS

- <img src="https://cdn.worldvectorlogo.com/logos/mysql-4.svg" width="25" height="25"/>    Mysql
 
- <img src="https://cdn.worldvectorlogo.com/logos/docker-4.svg" width="25" height="25"/>  Docker





# My Faculty Reg Portal

This is a Faculty Reg Portal that connects to a MySQL database. It uses Docker for easy deployment.

## Deployment

1. Clone the repository:

git clone https://github.com/akhandsinghjr/2201CS11_CS260.git
go to the proj1 folder


2. Build and start the containers: docker-compose up -d

This will build the Faculty Reg Portal image and start the MySQL and Node.js containers in detached mode.


3. Check the logs to ensure both containers are running: docker-compose logs -f

You should see the MySQL container initializing and the Faculty Reg Portal starting up.

P.S. as the node container server starts faster than the mysql container server please stop the node container once and then restart it


4. The Faculty Reg Portal will be available at `http://localhost:8000`.


## Configuration

The MySQL database credentials and other configuration settings are defined in the `docker-compose.yml` file. You can modify these values as needed.


## Notes

- The Faculty Reg Portal code is expected to be in the same directory as the `Dockerfile` and `docker-compose.yml` files.
- The MySQL data is persisted in a named volume (`mysqldb_data`), which will be created if it doesn't exist.
- The Faculty Reg Portal expects the MySQL database to be available at `mysqldb:3306`.
