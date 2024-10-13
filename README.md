# Next.js Application

This is a Next.js application that uses a MySQL database. To make the application ready for production, you need to set up a database and then deploy it, for example, on Vercel.

## Steps for Production

1. Install the dependencies using the command `npm install`.

2. Create a `.env` file in the root of the project and set the following environment variable:  
   `DATABASE_URL="mysql://<username>:<password>@<host>:<port>/<database>"`  
   Replace `<username>`, `<password>`, `<host>`, `<port>`, and `<database>` with the correct database values.

3. Once the database is ready, use Prisma ORM to generate the client and apply the migrations. Run the following commands:  
   `npx prisma generate`  
   `npx prisma migrate deploy`

4. Finally, after everything is prepared, you can deploy the application to Vercel or any other hosting platform of your choice.

The application is now ready for production.

---
