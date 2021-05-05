# Frontend login

Once you open the web frontend for your install, you will be greeted by a login screen. If this is your first time, you'll have to provide the web login credentials given to you by the installer script. Once you're inside the web frontend, you can create new users with your own passwords (see "about") at the end of this Frontend documentation category.

The default username for the web frontend upon install is `admin`. The password is randomly generated for every install and is only output in plaintext once by the install script.

These web frontend passwords are stored in the database, in `bcrypt` hash format using the `blowfish` non-cryptographically reversible algorithm.

Once a password is sent in the form with a post request, the check script will check the username and password on the system. If the user does not exist or you submitted a wrong username and password, you will be redirected back to the login form with an error message.

If the username exists on the `pcapanalyzer_creds` database inside of the `users` table, and the `bcrypt` hash matches the one calculated on the frontend form, you will be redirected to the PCAPAnalyzer frontend homepage.
