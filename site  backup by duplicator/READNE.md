    # How to use
        
    The following describes how to restore a site in the same or new location using a Duplicator package (installer/archive).  It's
    assumed you've created a package as described in the "Back up Site" section above and plan to install all files and the database contained in the package. _\* Items in green apply only to Duplicator Pro users._

    ### 1. Download package files to local computer After creating a package download the _installer and archive_ files from any one of the locations below to your local computer:   



    * **Default:** Click on the "Installer" and "Archive" buttons from the main packages screen to download.
    ---

    ### 2. Upload package files to target location

    Place the installer.php and archive.zip files in a directory where you would like to install/duplicate 	the WordPress site.   

    **ON A HOSTED SITE**   

        **INSTALLING IN AN EMPTY DIRECTORY (LITE AND PRO)**   
        [ Use FTP ](https://www.youtube.com/watch?v=Ci7iPXaKYQU) or [ cPanel ](https://www.youtube.com/watch?v=yvKwwYh2jr0) to upload both the archive.zip and installer.php to your host provider.
        Place the files in a new empty directory under your host's webroot where they are accessible from a valid url such as _http://your-domain/installer.php_ or _http://your-domain/your-wp-directory/installer.php_.
        On some hosts the root directory will be a something like _public_html_ &nbsp;-or- _www_.  If you're not sure what your root directory is then
        contact your hosting provider.   

        **Important:** Since the archive contains site customizations as well as core WordPress, WordPress shouldn't be in the directory beforehand. The only files in the directory should be the installer.php and archive before you run the installer.   


        **OVERWRITING EXISTING SITE (PRO ONLY)**   
         Duplicator Pro is capable of much faster installs when it's used to overwrite an existing site and reuses that site's database.   

        [ Use FTP ](https://www.youtube.com/watch?v=Ci7iPXaKYQU) or [ cPanel ](https://www.youtube.com/watch?v=yvKwwYh2jr0) to upload both the archive.zip and installer.php to your host provider 				 (place the installer.php and archive.php in the directory containing the existing site). The installer should be accessible from a valid url such as _http://{existing-site-domain}/installer.php_ or _http://{existing site-domain}/{your-wp-directory}/installer.php_.
        On some hosts the root directory will be a something like _public_html_ &nbsp;-or- _www_.  If you're not sure what your root directory is then
        contact your hosting provider.   


        _If you haven't chosen a hosting provider yet please see [host recommendations](https://snapcreek.com/wordpress-hosting/)._

       **ON YOUR OWN COMPUTER (localhost)**  

         Be sure you have PHP, Apache & MySQL installed on your local computer with software such as [XAMPP](http://www.apachefriends.org/en/xampp.html), [Instant WordPress](http://www.instantwp.com) or [MAMP](http://www.mamp.info/en/index.html) for MAC.
        Place the package.zip and installer.php into any empty directory under your webroot or where they can be
        served up by your local webserver then continue with Step 3 below.



    ---

    ### 3. Browse to installer.php and install

        1.   Open a web browser (i.e Chrome, Firefox, IE) and browse to the 'installer.php' file such as:  
             http(s)://your-domain/installer.php	or	http(s)://your-domain/your-wp-directory/installer.php.
        2.  On Step 1 ❯ Click the next button
        3.   On Step 2 ❯ Enter database setup info ❯ test connection ❯ click next   


            __ The vast majority of sitations require the 'server' field to be set to 'localhost'.  
            __ **If installing in an empty directory:** On database setup enter information for an existing empty database with no tables and a user with full rights to that database. You can easily ["__ Create A New Database and User"](https://www.youtube.com/watch?v=CHwxXGPnw48) or contact your host to have them set those up for you.  If you're not sure what information to use, just contact your host.  
            __ **If overwriting an existing site (Pro only):** When prompted to reuse database credentials on step 2, click Accept. This causes the database information from your existing site to be used in the install. **Important:** The database will be cleared so make sure you no longer need its data. If you need to preserve the old database then create a new one instead as [explained here](https://www.youtube.com/watch?v=CHwxXGPnw48).

            __ The Action "Connect and Remove All Data" will delete all tables to the database you connect to.   Be sure you're 100% of the
            sure of credentials	used when choosing this action.  For Duplicator Pro users consider
            using the "Connect and Back up any Existing Data" action if you're new to this process.  This will back up all the existing tables with
            a new prefix.
        4.  On Step 3 ❯ Click the next button
        5.  On Step 4 ❯ Login remove installer files
        6.  Your site has been migrated

    https://snapcreek.com/duplicator/docs/quick-start#quick-040-q
