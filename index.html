2020-July-27-ownCloud 10.5 Quickstart Guide.MARKUP
# **ownCloud 10.5 Quickstart Guide** 

# Software Requirements
ownCloud recommends the following software requirements for optimum performance, stability, support, and functionality. For more information, see [Deployment Considerations](https://doc.owncloud.org/server/10.4/admin_manual/installation/deployment_considerations) and [Deployment Recommendations](https://doc.owncloud.org/server/10.4/admin_manual/installation/deployment_recommendations.html).
## Environment
Table 1: Recommended Environment
| Platform  | Options |
| --- | ----------- |
| Operating system | Ubuntu 18.04 LTS |
| Database | MariaDB 10+ |
| Web server | Apache 2.4 with [prefork and mod_php](https://doc.owncloud.org/server/10.4/admin_manual/installation/manual_installation.html#multi-processing-module-mpm) |
| PHP runtime | 7.3 |   
Table 2: Other Supported Environments   
| Platform  | Options |
| --- | ----------- |
| Operating system | Debian 9 and 10 |
|  | Fedora 30 and 31 |
|  | Red Hat Enterprise Linux/Centos 7.5 and 8 |
|  | SUSE Linux Enterprise Server 12 with SP4 and 15 |
|  | Ubuntu 16.04 and 18.04 |
|  | openSUSE Leap 42.3 and 15 |
| Database | MySQL 8+ or MariaDB 10+; recommended |
|  | Oracle 11 and 12 |
|  | PostgreSQL 9 and 10 |
|  | SQLite; not for production |
| Web server | Apache 2.4 with prefork and mod_php |
| PHP runtime | 7.1, 7.2, and 7.3 |   
**Note**: For Linux distributions, ownCloud supports the latest two versions for each platform and the previous LTS version. 
## Hypervisors   
* Hyper-V   
* VMware ESX   
* Xen   
* KVM    
## Desktop Sync Client   
ownCloud recommends that you use the newest sync client with the latest server release. The latest stable client supports the following platforms:   
* Linux
  * CentOS 7.6+ and 8
  * Debian 9.0 and 10
  * Fedora 30, 31, and 32
  * Ubuntu 18.04, 19.04, 19.10, and 20.04
  * openSUSE Leap 15.0, 15.1, and 15.2
 * macOS X 10.10+; 64-bit only
 * Microsoft Windows 7+
## Web Browser
* Edge; current version on Windows 10
* IE 11 or later; except Compatibility Mode
* Firefox 60 ESR+
* Chrome 66+
* Safari 10+
## Mobile Apps
Use the newest mobile apps with the latest server release. The latest stable mobile apps support the iOS 9.0+ and Android 4.4+ platforms.
## Database Requirements
You require the following database settings to run ownCloud with a MySQL or MariaDB database: 
* Disabled, `BINLOG_FORMAT = MIXED`, or `BINLOG_FORMAT = ROW` configured Binary Logging.
* InnoDB storage engine. ownCloud does not support the MyISAM storage engine.
* `READ COMMITED` transaction isolation level      
For more information, see [Database Configuration on Linux](https://doc.owncloud.org/server/10.4/admin_manual/configuration/database/linux_database_configuration.html#mysql-mariadb-with-binary-logging-enabled).   
## Memory Requirements
The memory requirements to run an OwnCloud server vary according to the number of users and files, and the volume of server activity. ownCloud requires a minimum of 128 MB of RAM, but recommends you have 518 MB.   
# Installing ownCloud
1. Go to https://owncloud.org/download/   
2. On the Download ownCloud page, in the ownCloud server pane, click **Download Tar** or **Download Zip**. The file `owncloud-x.y.z.tar.bz2` or `owncloud-x.y.z.zip` downloads to your computer.
3. Download the `owncloud-x.y.z.tar.bz2.md5` or `owncloud-x.y.z.tar.bz2.sha256` checksum file.
4. Check that the MD5 or SHA256 checksum file is as follows:
```
md5sum -c owncloud-x.y.z.tar.bz2.md5 < owncloud-x.y.z.tar.bz2
sha256sum -c owncloud-x.y.z.tar.bz2.sha256 < owncloud-x.y.z.tar.bz2
md5sum  -c owncloud-x.y.z.zip.md5 < owncloud-x.y.z.zip
sha256sum  -c owncloud-x.y.z.zip.sha256 < owncloud-x.y.z.zip
```
5. Check the PGP signature:
```
wget https://download.owncloud.org/community/owncloud-x.y.z.tar.bz2.asc
wget https://owncloud.org/owncloud.asc
gpg --import owncloud.asc
gpg --verify owncloud-x.y.z.tar.bz2.asc owncloud-x.y.z.tar.bz2
```
6. Extract the archive contents from the files. Run the appropriate unpacking command for your archive type to unpack the file to a single ownCloud directory:
```
tar -xjf owncloud-x.y.z.tar.bz2
unzip owncloud-x.y.z.zip
```
7. Copy the ownCloud directory to its final destination. When you run the Apache HTTP server, you may safely install ownCloud in your Apache document root:
`cp -r owncloud /path/to/webserver/document-root`
where you replace `/path/to/webserver/document-root` with the document root of your Web server.
`cp -r owncloud /var/www`
**Note**: For other HTTP servers, we recommend that you install ownCloud outside of the document root.
# Configuring the Web server
The following procedures explain how to configure the web server with your system.
## Configuring Apache
1. For Debian and Ubuntu, create an `/etc/apache2/sites-available/owncloud.conf` file and enter the following code, where you replace the Directory and other file paths with your file paths:
``` 
Alias /owncloud "/var/www/owncloud/"
<Directory /var/www/owncloud/>
  Options +FollowSymlinks
  AllowOverride All

 <IfModule mod_dav.c>
  Dav off
 </IfModule>
</Directory>
```
2. Create a symlink to `/etc/apache2/sites-enabled` with the following code:
```
ln -s /etc/apache2/sites-available/owncloud.conf /etc/apache2/sites-enabled/owncloud.conf
```
## Additional Apache Configurations
1. ownCloud requires the module `mod_rewrite` to work. We recommend that you also enable the `mod_headers`, `mod_env`, `mod_dir`, `mod_mime`, and `mod_uniqe_id` modules. Run the following commands to enable the modules:
    * `a2enmod rewrite`
    * `a2enmod headers`
    * `a2enmod env`
    * `a2enmod dir`
    * `a2enmod mime`
    * `a2enmod unique_id`   

**Note**: To use the OAuth2 app, install and enable the `mod_headers` module.
2. Disable any server-configured authentication for ownCloud. If you turn on authentication on a parent folder, you can disable the authentication specifically for the ownCloud entry. After the Configuration file, in the <Directory section,  enter `Satisfy Any`. 
3. When you use SSL, take note of the ServerName. Specify a ServerName in the server configuration and in the CommonName field of the certificate. To enable access to your ownCloud through the internet, set both to the domain that you want to access your ownCloud server. 
4. Restart Apache with `service apache2 restart`.
**Note:** If you run ownCloud in a sub-directory and want to use CalDAV or CardDAV clients, configure the correct Service Discovery URLs.
## Configuring Apache Mod_Unique_Id

If you enable the module, ownCloud automatically includes the `UNIQUE_ID` environment variable to make the module available in the ownCloud log file. To check that the module works, complete the following steps: 
1. Run `phpinfo()` to check that the `UNIQUE_ID` environment variable is set.
2. Compare the value set for `UNIQUE_ID` in the output of `phpinfo()` with the value in the ownCloud log file to ensure that the two values match.   
## Enabling SSL
You can use ownCloud instead of plain HTTP, but we recommend that you use SSL/TLS to encrypt all of your server traffic, and to protect user logins and data in transit.
* When you install Apache under Ubuntu, it includes a simple self-signed certificate. To enable the SSL module and the default site, open a terminal and run:
```
a2enmod ssl
a2ensite default-ssl
service apache2 reload
```
## Multi-Processing Module (MPM)
* Make sure to use Apache prefork instead of a threaded MPM, such as event or worker with mod_php. 
## Running the Installation Wizard
After you restart Apache, run the Graphical Installation Wizard to complete the installation. 
1. Point your web browser to http://localhost/owncloud.
2. Enter your preferred administrator username and password.
3. Click **Finish Setup**.

**Note:** Set the directory permissions immediately after the installation completes. 

# Post-Installation Tasks
You can perform the following tasks when the installation completes to further configure the Web server. 

## Setting Strong Directory Permissions
When the installation completes, set the directory permissions immediately in your ownCloud installation. Make sure to set the directory permissions as strong as possible for greater security. After you set the permissions, the ownCloud server is ready for use. 

## Setting Headers
ownCloud has a mechanism to set headers programmatically. These headers are set with the `always` directive to avoid errors when there are additional headers set in the web servers configuration file, such as http.conf. For more information, see [mod_headers](https://httpd.apache.org/docs/current/mod/mod_headers).


## Managing Trusted Domains
In the config.php file, under the trusted_domains setting, add any URL that can access your server to a white-list. Users can log into ownCloud only when they point their browsers point to a URL that the trusted_domains settings lists. See the following example for a typical configuration: 
```
'trusted_domains' => [
   0 => 'localhost',
   1 => 'server1.example.com',
   2 => '192.168.1.50',
],
```
ownCloud automatically white-lists the loopback address 127.0.0.1; you can always log in if you have access to the physical server. If a load-balancer is in place and it sends the correct X-Forwarded-Host header, no issues occur. 

# Synchronizing ownCloud files to client machines
The ownCloud Client packages contain the owncloudcmd command line client that you can use to synchronize ownCloud files to client machines. owncloudcmd performs a single sync run to process the differences between client and server directories, propagates the files to bring both repositories to the same state, and exits the synchronization process. Contrary to the GUI-based client, owncloudcmd does not repeat synchronizations on its own nor does it monitor for file system changes. 
* To invoke owncloudcmd, use the following command to provide the local and the remote repository URL:
`owncloudcmd [OPTIONS...] sourcedir owncloudurl`
## Credential handling
`owncloudcmd` requires the user to specify the username and password using the standard URL pattern, for example:
```
$ owncloudcmd /home/user/my_sync_folder https://carla:secret@server/owncloud/remote.php/webdav/
```
To synchronize the ownCloud directory Music to the local directory media/music, through a proxy listening on port 8080, and on a gateway machine using IP address 192.168.178.1, the command line is:
```
$ owncloudcmd --httpproxy http://192.168.178.1:8080 \
              $HOME/media/music \
              https://server/owncloud/remote.php/webdav/Music.
```
# Creating a New User
**Notes:**
* The user's login name or username is their unique ID for ownCloud, and cannot change. 
* Login names may contain uppercarse or lowercase letters, numbers, dashes, underscores, periods, and @ symbols. After you create a user, you can enter their full name if it is different from their login name, or leave it blank for the user to complete. 
* The admin sets the new user's email. The user receives an email with instructions to set their password; both the user and the admin can change the user's password at any time.



1. In the ownCloud UI, enter the new user's login name and their email address. Optionally assign Groups membership.
2. Click **Create**.



# Connecting to the ownCloud Server through a Desktop 
* Install ownCloud on Mac OS X and Windows as follows: 
1. Go to https://owncloud.org/download/. 
2. Download the latest version of ownCloud that is appropriate for your operating system.
2. Double-click the application to launch the installation. 
3. Follow the instructions in the installation wizard. 
When the installation and configuration completes, the sync client automatically updates. 
* Install ownCloud on Linux as follows:
1. Go to https://owncloud.org/download/.
2. Follow the instructions on the download page to add the appropriate repository for your Linux distribution. 
3. Install the signing key.
4. Use the package manager to install the desktop sync client. 
Use the package manager to update your sync clients; the client displays a notification when an update is available.

**Note:** If you use Linux, enable a password manager so that the sync client can login automatically. 
# Connecting to the ownCloud Server through an iOS App
1. On your mobile device, open Safari, or any Web browser, and point it to your ownCloud server. 
2. Log in and go to your Personal page for a link to the ownCloud app on iTunes. 
3. Install and open the ownCloud app.
4. In the app, enter your ownCloud server URL and login. 
When the app connects to the ownCloud server, your Files page opens. For more information about how to use the iOS app, see https://doc.owncloud.org/ios/. 
# Connecting to the ownCloud Server through an Android device
1. On your mobile device, open a Web browser such as Chrome, Firefox, or Dolphin, and point it to your ownCloud server.
2. When you log in to your ownCloud account, a link for the ownCloud app in the Google Play Store displays. 
3. Click on the link to install and open the ownCloud app on your mobile device. 












































