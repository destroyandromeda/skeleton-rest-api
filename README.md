# express-rest-api

skeleton app on NodeJS
<pre>
1)Express
2)sequelize ORM
3)Postgres DB
</pre>

## Start project
#### Create new .env file based on .env.example and fill it

<pre>
<p><strong>npm i</strong>                       <small>//Install dependencies</small></p>
<p><strong>npm run pre-migrate</strong>         <small>//Create database if not exist in Postgres</small></p>
<p><strong>npx sequelize db:migrate</strong>    <small>//Run migrations</small></p>
<p><strong>npx sequelize db:seed:all</strong>   <small>//Run seeds with test data</small></p>
<p><strong>npm run dev</strong>                 <small>//Run project</small></p>
</pre>

### Routes
all routes start at /api

### Create migration
npx sequelize migration:generate --name %Name%


## Structure 
<pre>
src
 ┣ controllers
 ┃ ┗ *.controller.js
 ┣ database
 ┃ ┣ migrations
 ┃ ┃ ┗ *.js
 ┃ ┣ seeders
 ┃ ┃ ┗ *.js
 ┃ ┣ config.js
 ┃ ┣ createDB.js
 ┃ ┗ database.js
 ┣ models
 ┃ ┗ *.js
 ┣ routes
 ┃ ┣ index.js
 ┃ ┗ *.js
 ┣ app.js
 ┗ index.js
</pre>