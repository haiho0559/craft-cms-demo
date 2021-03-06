# craft-cms-demo
### how to run? 

1. Download/clone the repo on your computer:

   ```bash
   git clone https://github.com/haiho0559/craft-cms-demo.git
   ```

2. Run `composer install` within the clone:

   ```bash
   cd craft-cms-demo
   composer install
   ```

3. Copy the `.env.example` file at the root of the project to `.env`, and set its `DB_SERVER`, `DB_USER`, and `DB_PASSWORD`  variables to the correct values.
4. Ensure that the following files and directories have permissions that will allow PHP to read and write to them:

   - `.env`
   - `composer.json`
   - `composer.lock`
   - `config/license.key`
   - `storage/*`
   - `vendor/*`
   - `web/cpresources/*`

5. Create a new MySQL database called `craft-cms-demo`, and import `craft-cms-demo.sql` into it.

6. Create a new virtual host with the hostname `craft-cms-demo.test` that points to the `craft-cms-demo.test/web/` folder.

7. Edit your `hosts` file to resolve `craft-cms-demo.test` to `127.0.0.1`, if necessary.

Now point your browser at `http:///craft-cms-demo.test`. You should see the Craft CMS Demo homepage.

## Logging in

The Craft Control Panel is located at `http://craft-cms-demo.test/admin`. You can log in with the following credentials:

* Username: `admin`
* Password: `123456`
