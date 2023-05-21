----------------------------------------------

1. for database config edit `.env` file as below:
	
		DB_CONNECTION=mysql
		DB_HOST=db #this is mysql service name
		DB_PORT=3306
		DB_DATABASE=any_db_name
		DB_USERNAME=root
		DB_PASSWORD=password
	
----------------------------------------------

2. copy all your laravel project into `/src/`

----------------------------------------------

3. run this commands:

		docker-composer up
		
		docker exec -it laravel bash >
			composer update
			npm install
			npm run dev
			php artisan key:generate
			php artisan migrate
		
----------------------------------------------

4. run app & phpmyadmin like below:
		https://127.0.0.1:80 #app
		https://127.0.0.1:9000 #phpmyadmin
		
		
		
		