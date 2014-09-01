README

The readme for totroops.com

Should include setup instructions for the app.

You'll have to add a file, totroops/local_settings.py

This will point your local install at your local postgres database.

    # Settings for local host.
    import dj_database_url

    DATABASES = {
        'default': dj_database_url.config(default='postgres://<user>:<password>@localhost/<database>')
    }

Replace <user> <password> and <database> variables with credentials for your local database.
