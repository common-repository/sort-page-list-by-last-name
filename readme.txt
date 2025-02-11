=== Sort Page List by Last Name ===
Contributors: studiohyperset, oqm4, ryanajarrett
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=C2KQADH2TGTS4
Tags: wp_list_pages, page, function, list, title, plugin, name
Requires at least: 3.0
Tested up to: 5.4
Stable tag: 1.0

Sorts wp_list_pages-generated page lists by last name or, more generally, the last word of any page's title.

== Description ==

Aimed at archivists and other WordPress developers who use the names of individuals as page titles, this plugin sorts `wp_list_pages`-generated page lists by last name. More generally, the plugin can also be used to sort `wp_list_pages`-generated page lists by the last word of any page's title.

== Installation ==

After installing and activating, developers can order any `wp_list_pages`-generated page list by surname -- or, more generally, last word -- using the `sortbylastname=1` parameter, e.g., `<?php wp_list_pages('title_li=&sortbylastname=1'); ?>`. Use a "0" to (temporarily) disable the plugin. 

== Frequently Asked Questions ==

= Links =

* For feedback and help, visit: http://getsatisfaction.com/studio_hyperset/products/studio_hyperset_wordpress_plugins

* To learn about other Studio Hyperset WordPress plugins, visit http://studiohyperset.com/#solutions

* To help develop the Sort Page List by Last Name plugin, visit https://github.com/studiohyperset/sort-page-list-by-last-name

= Developer Notes =

PLEASE NOTE: Line 14 extracts each separate line of HTML from the original `wp_list_pages` output and puts it into an array called `$lines.` The `\n` parameter tells the explode command that each line ends with a carriage return. However, as of WordPress 3.2.1, the explode command assumes each line ends when it finds an `n`. As such, if developers edit the plugin using the WordPress code editor, they should add an extra backslash (`\`) in front of the `n` before saving the file (e.g, `$lines = explode("\\n", $val);`). The line will revert to `$lines = explode("\n", $val);` on save. 

Interested in helping develop the Sort Page List by Last Name plugin? Visit the GitHub repository: https://github.com/studiohyperset/sort-page-list-by-last-name

== Screenshots ==
&nbsp;

== Changelog ==

= 1.0 =
* 12/3/11 - Initial release

== Upgrade Notice ==

= 1.0 =
* 12/3/11 - Initial release
