---
layout: post
title: D8 Clearing the Cache
subtitle: by Mo Helmy
image: /img/logo-headless-drupal1.png
bigimg: /img/Drupal8.jpg
---

## Clearing the Cache Without Drupal 8 GUI <br/>

Using the rebuild script
Open settings.php (/sites/default/settings.php) in any text editor. Add this line to the end of the file and save it:

{: .box-error}
$settings['rebuild_access'] = TRUE;<br/>

{: .box-error}
Visit http://www.YourDomainName.com/core/rebuild.php 

In your browser (where www.YourDomainName.com is your site’s URL).<br/> 
After a short pause, you should be redirected to the home page of your site, and the cache should be rebuilt.<br/>
Open settings.php (/sites/default/settings.php) in a text editor.<br/>
Find the line you added with (( $settings[rebuild_access] )) remove this line, and save the file.<br/>
