# Instructions
To build your environment you just need to run 'docker-compose up --build' and this will build the following containers for you:
- php
- db
- webserver

You'll need to setup your own DB credentials which you can do by logging into your db container & logging into mysql using root access. You can then setup your own user & update the credentials in your docker-compose file there. For more information on how to do this please look at this Digital Ocean [article](https://www.digitalocean.com/community/tutorials/how-to-create-a-new-user-and-grant-permissions-in-mysql).

Please note that you shouldn't be including your db credentials in your docker-compose file. Please ensure they're safely stored in your environment specific .env file. 

Once built, you should be able to access this at http://localhost.

From here on, you can follow the Laravel [documentation](https://laravel.com/docs/8.x/installation).

# Database 

If you'd like to connect to your db container, please create a duplicate of the .env.example (or just rename it - please do not commit this). This file needs to be called '.env'. 
