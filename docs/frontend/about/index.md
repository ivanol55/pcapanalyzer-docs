# About PCAPAnalyzer

## developer credit and licensing

On the about page of PCAPAnalyzer you will find some information about the project, and some frontend management settings. First you can see information about the software version, licensing details, and developer credit.

## Identity and Access Management

You can also change the frontend page css for your session between the light and dark themes.

On the bottom of this page, you will find two identity and access management options: one to create and delete users to access the frontend webapp, and one for managing API secrets for API requests.

### User management

On this site, you can either create custom users and passwords to insert into the `pcapanalyzer_creds` database on the `users` table, or you can drop existing users under this form. Keep in mind, you are not allowed to drop all of the users on the system: there has to be at least one.

### API management

On this page you can generate new API keys, stored on the `pcapanalyzer_creds` database under the `apikeys` table, or drop API keys. If you want to, you can drop all of the API keys so no one has possible access to the API.
