For Prisma connection locally from docker:

npm install prisma

docker ps

start docker in your pc

Create schema for the postgres

DATABASE_URL=postgresql://postgres:mysecretpassword@localhost:5432/postgres

docker run -p 5432:5432 -e POSTGRES_PASSWORD=mysecretpassword -d postgres: to initialise database

npx prisma migrate dev: To create table in db
NOTE: You need call above command every single time, if u changing your schema file

npx prisma generate

     : to check data/table in localhost:5555

docker system prune -af : to clean the database for new start

3:52:00
