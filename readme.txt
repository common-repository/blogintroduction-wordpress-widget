=== Plugin Name ===
Contributors: KimHbel
Donate link: http://blog.huebel-online.de/
Tags: blog, introduction, sidebar, widget, thumbnail, snapshot
Requires at least: 2.1
Tested up to: 2.8
Stable tag: 0.3.0

Shows a thumbnail of a blogroll/linkroll-entry by random

== Description ==

This is a widget that brings up a little preview of a site into the sidebar. If you want to use this in a widget-less / static sidebar, give [blogintroduction-wordpress-plugin](http://wordpress.org/extend/plugins/blogintroduction-wordpress-plugin/ "blogintroduction-wordpress-plugin") a chance. The link is chosen by random out of the links in the WordPress link-manager. You can specify a single link-category or use all categories for the random-link-base.

You can also decide to show invisible/private links. This is for the case you want to show links as a preview you don't want to show in the linkroll.

If you want and if there is a description for the link done in the link-description-field it would be shown.

A refreshing via AJAX could be enabled with a specific time (in seconds) when the next thumbnail would be loaded.

This widget uses the [websnapr](http://www.websnapr.com/ "Website Thumbnais For Your Site")-Service for generating the thumbnail-images. Keep their [term of use](http://www.websnapr.com/terms/ "General Terms and Conditions for Websnapr") in mind. You should get an API-Key for free from there to use this widget and get more then 80 snapshots per hour, with key it would be about 340 per hour (250.000 a month).

Since Version 0.3.0 you could also use the image-link stored in the link-manager for containing the link to the preview-image. If no link is given the widget would use websnapr as fall back.

If you want to translate the plugin, feel free to do it! Since Version 0.2.0 the Output is fully internationalized.

To see the widget working in a production-environment, visit the [author's blog](http://blog.huebel-online.de/ "Blog of Kim Huebel").

If you want to leave a feedback, feel free to do this on the [plugin's homepage](http://blog.huebel-online.de/blogintroduction-wordpress-widget/ "Home of blogintroduction-wordpress-widget - Blog of Kim Huebel") of the author's blog. Though the pages are in german, comments in english are wellcome, too.

== Installation ==

1. Upload `blogintroduction.php` and `blogintroduction_ajax.php` to the `/wp-content/plugins/blogintroduction-wordpress-widget` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Go to Presentation -> Widgets and add the Blogintroduction widget
4. Configure your widget

The configuration is a simple thing:

* Title: This is simple the title of the sidebar-box shown in the box-header.
* Websnapr-API-Key: Here you could put in your API-Key. It's not necessary to fill this field for running the widget but its better to keep in mind with the [term of use](http://www.websnapr.com/terms/ "General Terms and Conditions for Websnapr") I think.
* Image-width: The value is a the number of pixels of the image-width in the sidebar. This parameter correspondents to the width-value in the html-img-tag.
* Image-height: The value is a the number of pixels of the image-height in the sidebar. This parameter correspondents to the height-value in the html-img-tag.
* use4:1-ratio: If checked, height would be well-sized to a 4:3-ratio corresponding to the width-value. Given height above would be ignored then.
* Image-source: Here you could chose from where the preview-image would be loaded: From websnapr or from a location given by the Image-URL in the link-manager.
* Link-category: Here you could chose the category of the links that would be the source for the random-links.
* Link-target: Simply means link-target. So where the link should be opened. "Im neuen Fenster" means in a new window, "Im aktuellen Fenster" means in the actual window of the browser.
* Show description: If the checkbox is checked, the link-description in the link-manager would be shown with a Label "Description" (depending on the translation).
* Show private links: Check this box to show private-links.
* Show new thumbnail in ... seconds: Here you enable the auto-renew-function, that means, every x seconds depending on the value you enter in the box on the right side, a new thumbnail would be shown. The minimum time is 10 seconds to avoid heavy traffic and other problems.

== Screenshots ==

1. This is the output of the widget, as you see it on the sidebar.
2. This is the widget-configuration-dialogbox.

== Changelog ==

Version 0.3.0:
* Image-Source chooseable
* Fixed issue with image-height

Version 0.2.3:

* Fixed issue with malfunctional refresh

Version 0.2.2:

* Fixed html-output for IE (description-part)

Version 0.2.1:

* Referer-check in AJAX-part implemented
* Output now validates against W3C

Version 0.2.0:

* plugin-internationalization included

Version 0.1.2:

* minimum refresh time set to 10 seconds

Version 0.1.1:

* plugin activation fixed

Version 0.1.0:

* adding AJAX for refreshing thumbsnails

Version 0.0.2:

* API-Key added
* show private/invisible links added
* CSS-Style-Classes added
* urlencoding fixed

Version 0.0.1:

* Initial shot.

== Frequently Asked Questions ==
= Where could I leave a comment or a question relating the plugin? =

If you want to leave a feedback, feel free to do this on the [plugin's homepage](http://blog.huebel-online.de/blogintroduction-wordpress-widget/ "Home of blogintroduction-wordpress-widget - Blog of Kim Huebel") of the author's blog. Though the pages are in german, comments or questions in english are wellcome, too.

= Sometimes I see thumbnails containing an error 404 or "bad request" or something, what's about this? =

If you see thumbnails containing some errors the cause lies at websnapr itself. I don't know, how they produce the thumbnails but it's not in my hands to fix this subject.
