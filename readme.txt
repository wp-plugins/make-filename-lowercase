=== Make Filename Lowercase ===
Contributors: ereckers
Donate link: http://www.kliky.com/make-payment/
Tags: strtolower, lowercase, filename, media, upload, sanitize_file_name, strtolower filename, lowercase filename, strtolower media, lowercase media, strtolower upload, lowercase upload
Requires at least: 3.0.1
Tested up to: 3.0.3
Stable tag: 1.0.0

Sets uploaded media filename to lowercase.

== Description ==

Sets uploaded media filename to lowercase as filter on sanitize_file_name. Based on post at Stack Overflow asking if there is a way to "Rename files during upload within Wordpress 3.0 backend".

Created for WordPress 3.0.1+ which saves any uploaded media filename (Image, Video, Audio) as lowercase. This effectively changes the name of the file at upload if a user were to upload a file with any uppercase characters.

For instance:

* MOVIE-FILE.MOV > movie-file.mov
* Movie-File.wmv > movie-file.wmv
* ImAgEfILe.gif > imagefile.gif
* imageFile.JPG > imagefile.jpg
* ETC > etc

* Note: WordPress sets file extension to lowercase. This plugin does a strtolower on the filename.

== Installation ==

1. Download the plugin and unzip it.
2. Upload the folder /make-filename-lowercase to your /wp-content/plugins/ folder.
3. Activate the plugin from your WordPress admin panel.
4. Installation finished.

== Screenshots =

1. Upload a media filename of mixed case (in this case, the file MIXED-cAsE-filename.JPG).
2. You'll see that the filename has been changed to all lowercase (mixed-case-filename.jpg) while preserving the case for the Title.
3. A image detail view from the Media Library showing the new File name as lowercase.

== Frequently Asked Questions ==

= Why was this plugin created? =

This plugin evolved from a client requirement that all uploaded media filenames contain no uppercase characters.

= Why did you release this plugin? =

It was useful to me and I wanted to work through the process of releasing a WordPress plugin.

= Why shouldn't this just be added to a theme's functions.php file? =

Upgradeability, portability, backwards compatibility, and other *abilities. If for some reason this function were in need of customization due to a WordPress version upgrade, the plugin will be centrally responsible for releasing the fix as opposed to updating the theme(s).

== Changelog ==

= 1.0.0 =

* Initial release

== Upgrade Notice ==

