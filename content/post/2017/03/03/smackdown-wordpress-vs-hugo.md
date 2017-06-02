+++
Description = "Smackdown: WordPress vs Hugo"
menu = "main"
Categories = ["technology", "development"]
date = "2017-03-03T10:56:07+02:00"
title = "smackdown: wordpress vs hugo"
Tags = ["technology", "hugo", "smackdown"]
ogimage = "http://www.moveableonline.com/Assets/wordpress-logo.png"
metadescription = "WordPress is a hugely popular platform, but is it always the right thing to use? Take a look at this smackdown comparison between WordPress and Hugo, a static site generator."
+++

<img width="45%" src="http://www.moveableonline.com/Assets/wordpress-logo.png">
<img width="45%" src="http://themes.gohugo.io/img/hugoSM.png">

The question today is:

Which is a better platform in terms of:

* Speed
* Security
* Infrastructure Requirements
* Flexibility

between WordPress and Hugo.

### what is wordpress?

WordPress is, by volume, the leading web site creation engine in the world, powering an impressive [25% of all web sites](http://venturebeat.com/2015/11/08/wordpress-now-powers-25-of-the-web/). It's based on PHP and MySQL. It serves pages dynamically.
Upon each request, WordPress will get information from the database, and build the page using a combination of the data, the WordPress
theme and plugins, and the WordPress engine itself.

### what is hugo?

[Hugo](https://www.gohugo.io) is the 2nd most popular static site generator. It is known for lightning fast speed, being written in Go,
and pre-generates all of the pages of a given project. This means that the pages are not served dynamically, but rather statically. The
entire site is rebuilt when a change is made, and the static assets are re-deployed.

### how do they stack up?

#### Speed

WordPress serves pages dynamically, meaning that every time a request is made to the server, the user must wait for the WordPress engine
to fetch data from the database, and wait for the page to be built by the server side scripts that make up a WordPress instance, which
can be effected by multiple plugins and PHP scripts.

Since this is a multi step process, it will impact page load speed.

![Static vs dynamic web sites](http://www.udeserve.in/blog/wp-content/uploads/2013/10/Static-vs-dynamic-website.jpg)

Hugo, on the other hand, pre-generates everything based on HTML layouts, Go HTML template logic and content files. Since the result is
static HTML, there is no wait for the page to be generated before it's served - it can just be served.

Although there are ways to speed up WordPress page load speed, such as minifying assets and moving load blocking scripts
from the header to the footer, these apply to Hugo as well.

WordPress has a range of caching plugins available which can help, but the clear winner is Hugo.

I contribute to a WordPress based blog called [The Men-Tal Hospital](http://www.thementalhospital.co.za). I did a comparison between load times of the two sites using the [Pingdom Website Speed Test](https://tools.pingdom.com).

The Men-Tal Hospital took an average of 14 seconds to load.
Raen, based on Hugo, took merely 0.68 seconds.

WordPress is smacked down hard here. **Running total: Hugo 1, WordPress 0**

#### security

WordPress has a bad [security track record](https://premium.wpmudev.org/blog/wordpress-security-exploits/), and it's partially due to the fact that it relies
on a rather large technology stack - a web server, MySQL database, PHP installation, a WordPress instance, and then whatever plugins and themes are used to
achieve the final web site build. If any of these technologies in the stack of vulnerable, it could cause a security breach. This is before considering the
fact that every area where user input is allowed and talks to the WordPress instance and database adds to the attack surface area.

Hugo sites, on the other hand, are statically built, and have a far smaller attack surface area.

There's no real competition in this area - Hugo smacks down WordPress again. **Running total: Hugo 2, WordPress 0**

#### infrastructure requirements

WordPress requires a large technology stack: a web server, PHP, and MySQL. It is also recommended that the operating system is Linux. I don't have a problem
with this, as I love Linux, but the truth is that it does narrow down your hosting choices somewhat. It also means that there's a lot more maintenance involved
in terms of software updates. The OS, database, WordPress and PHP installation must all be kept up to date. This can cause incompatibilities and errors to
creep in and unless handled carefully, could become a headache.

Hugo just requires a web server, as the entire site is static. Sites built with Hugo can be deployed directly on CDNs and are great choices for deploying to
Cloud based services such as S3 or Azure.

It's another hard smackdown. **Running total: Hugo 3, WordPress 0**

#### flexibility

WordPress is very flexible at the surface level - themes can be spun up quickly which can change the look and feel of the site in short order. Plugins can
be used to add almost any functionality you desire. The problem comes in when too many plugins are added, or themes become too complicated and
conflict with other parts of the system. There's no question that you can add functionality very easily to WordPress, as you can drop in PHP scripts
quite easily if all else fails - but often you will do this at your peril, as WordPress over-customization can cause serious issues on your site.

Hugo is flexible in a different way. It's not so easy to make surface-level changes, but mid-level changes are much easier in Hugo, as almost all
changes can be made with HTML, Go HTML templates, and content files. WordPress is a bit more flexible in some ways, as if interactive elements need to
be added that require server side scripts, AJAX will have to be employed to get the functionality into a Hugo-based site, and if too many of these
elements are required, Hugo is no longer a good choice.

WordPress wins this one, but narrowly. **Running total: Hugo 3, WordPress 1**

### conclusion

If you require a lot of server-side code, Hugo may not be the right choice for you, but the reality is that most sites that WordPress and Hugo are used
for do not require this functionality. Everything from site search (JSON based indexes and Google Custom Site Search) to forms (Marketing automation tools like Hubspot or Mautic) can be handled without server-side code, with better results in most cases.

The speed, infrastructure and security advantages of using Hugo far outweigh any surface-level ease of use benefits that WordPress provides.

Hugo wins this smackdown.
