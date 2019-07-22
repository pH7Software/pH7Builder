# 🚀 pH7Builder 😍

## ⚡ 2019 KILLER Dating WebApp Builder Software!

[![PayPal](https://img.shields.io/badge/Donate-PayPal-lightgrey.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=X457W3L7DAPC6 "Help keep me off the streets! ;)") [![Build Status](https://scrutinizer-ci.com/g/pH7Software/pH7-Social-Dating-CMS/badges/build.png?b=master)](https://scrutinizer-ci.com/g/pH7Software/pH7-Social-Dating-CMS/build-status/master) [![GPL v3 Licence](https://img.shields.io/aur/license/yaourt.svg)](https://opensource.org/licenses/gpl-3.0.html) [![SourceForge](https://img.shields.io/badge/Download-SourceForge-orange.svg)](https://sourceforge.net/projects/ph7socialdating/files/latest/download) [![Patreon](https://img.shields.io/badge/Subscribe-Patreon-red.svg)](https://www.patreon.com/bePatron?u=3534366 "Become a Patron Today!")

**pH7Builder, Dating Solution™** gives a **Professional**, **Free** and **Open Source** Enterprise-Class Dating WebApp CMS, fully responsive design, low-resource-intensive, powerful and very secure.

![Professional PHP Social Dating Builder Software](https://cloud.githubusercontent.com/assets/1325411/19419476/5475b32c-93d0-11e6-9756-8e7db8df129f.png)

🤔 *Imagine in 3 months' time..., you have a well-known successful online community with thousands of satisfied users, and without spending a dime for it.*
*Instead, you spent money on advertising, user acquisition and other marketing strategies.*
*Imagine the time you have saved. The great business and freedom you have now built.*

With **[pH7Builder](https://sourceforge.net/projects/ph7socialdating/files/latest/download)**, *THIS IS TOTALLY POSSIBLE!* (however, you have to be motivated! Nothing comes as magic).


![pH7Builder allows anyone to start a web dating app like Tinder/Bumble or Badoo](https://cloud.githubusercontent.com/assets/1325411/19419477/5476b45c-93d0-11e6-823d-d293f186c0f7.png)


## 👀 pH7Builder's Overview

**pH7 Dating CMS** is a **Social/Dating CMS** written in **Object-Oriented** PHP (*OOP*), fully compatible and highly optimised for PHP 7+ and based on **MVC** architecture (Model-View-Controller).

It is designed with the **KISS** principle in mind, and the whole source code can be read and understood in minutes. For a better flexibility, the software uses **PDO** (PHP Data Objects) abstraction which allows the choice of the database. The principle of development is **DRY** (Don't Repeat Yourself) aimed at reducing repetition of information of all kinds (no duplicate code) and **YAGNI** principle to avoid unused code/not needed functionality in the software.

This Free and Open Source **Social Dating Site Builder** wants to be low resource-intensive, powerful, stable and secure. The software also comes with 42 system modules and is based on **pH7Framework** *(written specifically for this project)* that has over 52 packages.

*To summarize, **pH7Builder** gives you **the perfect ingredients** to create the **best online dating service** or **social networking** website on the World Wide Web!*

![Build a Social Dating Web App with pH7Builder](https://cloud.githubusercontent.com/assets/1325411/19419481/657386a4-93d0-11e6-8eee-95deba2d30a0.png)


## 👨‍🍳 The Cook

[![Pierre-Henry Soria](https://avatars0.githubusercontent.com/u/1325411?s=200)](https://pierrehenry.be "My personal website :-)")

Coded & Designed with lots of ❤ by [Pierre-Henry Soria](https://ph7.me). A SUPER Passionate Belgian Software Engineer 🍫🍺

You can reach me at *pierre {AT} soria {D0T} email*


## 🤝 Hire Me At Your Company?

Do you need a software engineer like me (and willing to relocate) at your company..? **[Let's chat together](https://www.linkedin.com/in/ph7enry/)**! 😊


## 💲 Offer Me A Cup of Tea? (...or tea bags...) 🍵

You appreciate the project, the several years I spent on it, and don't want to let it die...?

[![Paypal](templates/system/modules/ph7cms-helper/themes/base/img/paypal-donate.en.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=X457W3L7DAPC6)
[![Patreon](templates/system/modules/ph7cms-helper/themes/base/img/support-patreon.en.png)](https://www.patreon.com/bePatron?u=3534366 "Become a Patron")


## ⚙ Technical Requirements

* **Server** Apache with mod_php or with PHP in CGI, FastCGI mode (nginx, LiteSpeed and IIS should also work. You might have to change some pieces of code and change the URL rewriting to make it work).

* **Application Server** PHP 5.6 or higher (recommended version: **PHP 7.0.4** or higher).

* **Database** MySQL/MariaDB 5.5.3 or higher.

* **URL rewriting extension** [Apache](https://ph7cms.com/doc/en/how-to-install-rewrite-module), nginx, LiteSpeed, IIS (for Web.config, you have a [good tutorial here](https://web.archive.org/web/20190116102700/http://www.phpgenious.com/2010/04/url-rewriting-with-php-and-iis-7/)).

* **Specific Requirement** Server has to be connected to Internet.

* **Minimum Web Space** 2.0 GB

* **Video Module Requirement (only if enabled)** [FFmpeg](https://ffmpeg.org)


## 🛠 Installation

  * Github:
    * Clone pH7Builder from Github `git clone git@github.com:pH7Software/pH7Builder.git`
      (use `--depth=1` if you don't need the history)
    * [Install Composer](https://getcomposer.org/doc/00-intro.md)
    * From a command line opened in the folder, run `composer install` to install pH7Builder's dependencies.
  * Composer:
    * [Install Composer](https://getcomposer.org/doc/00-intro.md)
    * `composer create-project ph7software/ph7cms --prefer-dist ph7builder`
  * Sourceforge:
    * Directly download the latest stable version from [Sourceforge](https://sourceforge.net/projects/ph7socialdating/).
  * Softaculous:
    * If your Web host offers Softaculous, you might be able to install [pH7Builder in one-click with Softaculous](https://www.softaculous.com/apps/socialnetworking/pH7Builder).


## 🏗 Nginx Specification (configuration)

In order to get pH7Builder working on nginx server, you need to add some custom nginx configuration.

Create `/etc/nginx/ph7builder.conf` and add the following:

```nginx
location / {
    try_files $uri $uri/ /index.php?$args;
    index index.php;
}
```

*Please note that the above code is the strict minimum and obviously you can add more rules by comparing with the [main Apache .htaccess file](https://github.com/pH7Software/pH7Builder/blob/master/.htaccess).*

Finally, in your nginx server configuration, you will have to include `ph7builder.conf` file to complete the configuration like below:

In file, e.g., *`/etc/nginx/sites-enabled/yoursite.conf`* for Ubuntu and other OS based on Debian or `/etc/nginx/conf.d/yoursite.conf` for CentOS and other OS based on Red Hat.

```nginx
server {
    # Port number. In most cases, 80 for HTTP and 443 for HTTPS
    listen 80;

    server_name www.yoursite.com;
    root /var/www/ph7builder_public_root;
    index index.php; #you can use index.ph7; for hidding the *.php ...
    client_max_body_size 50M;

    error_log /var/log/nginx/yoursite.error.log;
    access_log /var/log/nginx/yoursite.access.log;

    # Include ph7builder.conf. You can also directly add the "location" rule instead of including the conf file
    include /etc/nginx/ph7builder.conf;
}
```

For more information, please refer to the nginx documentation.
<br />

![Create Your Own Niche Dating Service in New York City](https://cloud.githubusercontent.com/assets/1325411/19419480/65738a1e-93d0-11e6-9fbe-a48fa36fc53a.png)


## 📝 Translations

You can find and add other languages on the [I18N repo](https://github.com/pH7Software/pH7-Internationalization).


## 📚 Documentation

[pH7Builder Documentation](https://ph7cms.com/doc/)


## 💖 Contributing

![I Love Open Source](static/img/love-open-source-logo.png)

Anyone can contribute on **[pH7Builder GitHub](https://github.com/pH7Software/pH7Builder)** repository!

Finding bugs, improving the CMS/doc or adding translations. Any contribution is welcome and highly appreciated!

Just clone the repository, make your changes and then make a push ;-)

*WARNING: Your code/modification must be of excellent quality and follow the [Code Convention](https://ph7cms.com/doc/en/code-convention) and [PSR](https://www.php-fig.org/psr/).* I manually review and validate all improvements and changes you I've done.


![Beautiful Profile Dating Page](https://user-images.githubusercontent.com/1325411/35779585-68f0d5fc-09c7-11e8-91eb-bf793fcfab6e.png)


## 🌲 pH7Builder; The Eco-Friendly CMS ❤️

![Eco Friendly. Love the World and Love the Nature](static/img/love-nature.svg)

[pH7Builder](https://ph7cms.com) has been built to reduce the power and CPU usage of your server in order to preserve the nature and help to save our environment.

pH7Builder's templates also use lighter colors since LCD monitors use less electricity to display them.

Finally, **please consider using green Web hosting** (which use Green Power supply).


-> Other [10 Easy Ways to Green Your Social Community](https://mashable.com/2010/01/01/green-your-web-site/) 😉 <-


## ⚖ License

**pH7Builder** is generously distributed under **Open Source, Free** License.

[General Public License 3](https://www.gnu.org/licenses/gpl.html) or later; See the *PH7.LICENSE.txt* and *PH7.COPYRIGHT.txt* files for further details.


![Admin Panel, Browse Users](https://cloud.githubusercontent.com/assets/1325411/14080251/b476e5c6-f4fb-11e5-825e-ddc992ba1055.png)
