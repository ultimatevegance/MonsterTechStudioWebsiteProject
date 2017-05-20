# how to run on local development environment
* first composer update: run `composer install`  to install all the dependencies 
* then set up database connection :open up the .env.example and edit this line:

  ```
  DB_CONNECTION=mysql
  DB_HOST=127.0.0.1
  DB_PORT=3306
  DB_DATABASE=homestead
  DB_USERNAME=your_username
  DB_PASSWORD=your_password
  
  ```
  After that, save it as .env file. This is Important!
  
* setup the key :this one is simple, but make sure you've done step 2 above, which is renaming the file.
	
   ```
    $ php artisan key:generate

   ```
    and Laravel will automatically generate random key for you.
* run the website app 

    ```
    $ php artisan serve

    ```
