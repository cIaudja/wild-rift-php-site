# Wild Rift fan site

A website about the mobile game League of Legends: Wild Rift, built in 2022 as my final-year high school project. It uses plain PHP with a MySQL database, plus HTML, CSS and some JavaScript.

## Features

- Home page and game overview
- List of champions, with a page for each one and a quiz
- Sign-up, login and profile editing
- Skin shop with an in-site coin balance and a simulated payment flow
- Support form

## How to run it locally (macOS)

### 1. Install and start XAMPP

1. Download XAMPP for macOS from [apachefriends.org](https://www.apachefriends.org/) and install it.
2. Open the **XAMPP** app (in `Applications/XAMPP/manager-osx`).
3. Go to the *Manage Servers* tab and start **Apache Web Server** and **MySQL Database**. Both should turn green.

### 2. Copy the project into XAMPP

The site expects to live in a folder called `Progetto` inside XAMPP's `htdocs` folder:

```bash
git clone https://github.com/cIaudja/wild-rift-php-site.git /Applications/XAMPP/xamppfiles/htdocs/Progetto
```

(Or download the ZIP from GitHub, unzip it, rename the folder to `Progetto` and move it into `/Applications/XAMPP/xamppfiles/htdocs/`.)

### 3. Create the database

1. Open [http://localhost/phpmyadmin](http://localhost/phpmyadmin).
2. Click the **Import** tab at the top.
3. Choose the file `wildrift.sql` from the `Progetto` folder and click **Import** (or **Go**) at the bottom.

This creates the `wildrift` database with all its tables. The PHP code connects as `root` with no password, which is the XAMPP default, so nothing needs to be configured.

### 4. Open the site

Go to [http://localhost/Progetto/home.php](http://localhost/Progetto/home.php).

When you are done, stop Apache and MySQL from the XAMPP app.

## Notes

- The images are not included in the repository because of their size, so some pages will show missing images.
- The `non attivi` folder contains old versions of some pages that are no longer used.
