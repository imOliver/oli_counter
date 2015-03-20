# oli_counter

## Description
jQuery plugin countdown to / from a given date / time

## Setup
Download the plugin archive, extract ".js" files to a folder with javascript files in your project.
Connect plugin in your HTML file:
```
<script src="your_javascript_folder/jquery.oli_counter-0.5.js" type="text/javascript" charset="utf-8"></script>
```
Insert HTML block for counter:
```
<div class="counter" data-end="YYYY,MM,DD,HH,MM,SS"></div>
```

To create and start default counter:
```
$('.counter.wd').oli_counter();
```
To create and start counter with options:
```
$('.counter.wd').oli_counter({
	'times_array': Array(1, 60, 3600),
	'animation_speed':100
});
```
To stop counter:
```
$('.counter.wd').oli_counter('destroy');
```

You can tune the counter with options:
* **times_array** - an array of integers, each of which specifies the group size counter in seconds. By default the numbers are 1, 60, 3600, 86400, 2629800, 31557600. If you want to show 3 groups of numbers "minutes", "hours", "days" this array must consist of 60, 3600, 86400. 
* **group_text** - an array of strings, which specifies the groups titles. By default: 'seconds','minutes','hours','days','months','years'. Note, that you MUST change this option if you change 'times_array' from default. You can also use this option for localization of the plugin. 
* **refresh_speed** - counter refresh rate in milliseconds. By default: 500.
* **animation_speed** - numbers animation speed in milliseconds. By default: 500.

## Requirements

### Mandatory requirements
* [jQuery](https://jquery.com/) v. 1.6+

## Browsers

### Desktop browsers
The plugin is regularly tested with the latest browser versions and supports the following minimal versions:

* Google Chrome
* Apple Safari 4.0+
* Mozilla Firefox 3.0+
* Opera 11.0+
* Microsoft Internet Explorer 8.0+

### Mobile browsers
The File Upload plugin has been tested with and supports the following mobile browsers:

* Google Chrome on Android 4.0+
* Default Browser on Android 2.3+

## License
Released under the [MIT license](http://www.opensource.org/licenses/MIT).

## Donations
oli_counter is free software, but you can donate to support the developer, Anton Grichenko:

PayPal: [![PayPal](https://www.paypalobjects.com/WEBSCR-640-20110429-1/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=AD8MHRP3GET5G&lc=RU&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted)
