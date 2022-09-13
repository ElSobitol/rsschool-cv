# Personal Curriculum vitae

![мое фото](my_face.png)


## My name is Vitali Mayerau

* __29 years old__
* __Contacts e-mail:__ maerovv34@gmail.com
* __Social Network:__
https://www.linkedin.com/in/vitalimayerau/

* __Discord:__ @elsobitol

<br><br>

## Actual info:

I have more than 3 years of experience in the IT industry. I started creating the first websites in 2014, temporarily stopped in 2016, continued since 2019. I work on projects in various fields, taking part mainly in the development of the frontend development (until 2021), now I am trying to delve more into the backend. I am always interested in learning new technologies, improving my skills and finding optimal solutions for various tasks.
<br>

__Strengths include:__
* WordPress development (creation of the first projects since 2014)
* Solving technical problems and teamwork
* Visual layout on Elementor
* Setting up payment systems in WooCommerce
* Working with WordPress plugins and templates, changing existing solutions.


## Areas of Expertise

### __Programming languages:__
	HTML, CSS; just a little bit PHP, C# (simple console app), Python (simple console app from terminal)
### __Technologies:__
	WordPress, DLE, Joomla, Elementor, WooCommerce, Bootstrap, ACF, CPT UI, Python, Flask/Jinja, Alice Yandex, Json		
### __Databases:__
    MySQL, SQLite		
			
### __IDE and tools:__
	IntelliJ IDEA, Brackets, Visual Studio, Notepad++, Sublime Text, Atom, PhpStorm, Pycharm Community and Pro, Visual Studio Code, Git Bash 		

### __Operating systems:__
	Windows		

### __Project tracking and bug tracking systems:__
	Github, Jira.		

### __Backup site systems:__
	Akeeba, Duplicator, WPvivid, Git	
### __Foreign Languages:__
    Intermediate level of English
    Elementary level of Ukrainian



# Code Examples(CodeWars)

```php
function multiply($a, $b) {
  return $a * $b;
}
```

```php

abstract class Card
{
    public $title;
    public $subtitle;
    public $price;
    public $size;

    public function __construct(string $title, string $subtitle, int $price, int $size)
    {
        $this->title = $title;
        $this->subtitle = $subtitle;
        $this->price = $price;
        $this->size = $size;

    }

}

class SecondCard extends Card
{
    public $weight;
    public function __construct(string $title, string $subtitle, int $price, int $weight)
    {
        $this->weight = $weight;
        parent::__construct($title, $subtitle, $price, $weight);
    }
}

class ThirdCard extends Card
{
    public $dimension;
    public function __construct(string $title, string $subtitle, int $price, string $dimension)
    {
        $this->dimension = $dimension;
        parent::__construct($title, $subtitle, $price, $dimension);
    }
}
```

```python

from flask import Flask, request
import logging
import json
import random

app = Flask(__name__)

logging.basicConfig(level=logging.DEBUG)

#Создаем запрос на корневой адрес, используем метод POST
@app.route('/', methods=["POST"])
def start():
    logging.info(request.json)
    spisok_citat_1_vopros = ["Очевидно, что ничего не очевидно!", "Здорово, бандиты!", "Где деньги, Лебовски?"]
    citata_velikih = ["Счастье - это не обладание тем, чего желаешь, а желание того, чем обладаешь.", "Чудеса - там, где в них верят, и чем больше верят, тем чаще они случаются.", "Веди себя так, будто ты уже счастлив, и ты действительно станешь счастливее."]
    bye = ["Уже уходите? Очень жаль.", "До скорой встречи", "Буду с нетерпением вас ожидать вновь"]
    response = {
        "version": request.json["version"],
        "session": request.json["session"],
        "response": {
            "end_session": False

        }
    }

    req = request.json
    if req["session"]["new"]:
        response["response"]["text"] = "Привет! Какую цитату тебе вывести?"
    else:
        if req["request"]["original_utterance"].capitalize() in ["Для важных переговоров"]:
            response["response"]["text"] = random.choice(spisok_citat_1_vopros)
        elif req["request"]["original_utterance"].capitalize() in ["Цитата великих"]:
            response["response"]["text"] = random.choice(citata_velikih)
        elif req["request"]["original_utterance"].capitalize() in ["Спасибо", "Пока", "Увидимся"]:
            response["response"]["text"] = random.choice(bye)
            response["response"]["end_session"] = True

    return json.dumps(response)

```

# Experience

## March 2022 – April 2022
### Technical Specialist & Developer
* __Project:	Website refinement based on WordPress. Ecosota Project__. 

* __Team:	1 Technical Specialist(Me).__
* __Participation:	Setting up on the site, using PHP hooks and ACF.__
* __Tools and technologies:	PHP 7.4 – 8.0, MySQL old version, WP Hooks, ACF, plugins WordPress.__

## December 2021 – Present
### Technical Specialist 
* __Project:__	Technical support for the Accelerator Optimization plugin for WordPress, search and help in compatibility with gallery and slider plugins.
* __Team:__	1 Technical Specialist
* __Participation:__	Setting up plugin optimization on third-party client sites. Creating css exceptions in accelerator settings
* __Tools and technologies:__	PHP 7.4 – 8.0, MySQL old version, Elementor, CSS, seraphinite accelerator, WordPress

## September 2021 – November 2021
### Developer
* __Project:__	Website refinement based on WordPress. TVG Project.  With WooCommerce
* __Team:__	1 Developers, 1 Technical Specialist
* __Participation:__	Setting up on the site, create new functions on PHP, using PHP hooks.
* __Tools and technologies:__	PHP 7.4 – 8.0, MySQL old version, WP Hooks, WooCommerce, WordPress, Gutenberg editor.


## March 2021 – August 2021
### Developer
* __Project:__	Website development based on WordPress. Experience in developing sites realties with using ACF plugin and custom fields. Creating projects on WordPress + Elementor, using ACF + CPT UI + Crocoblock Jet Widgets(landing pages and full-fledged sites). Using the plugin «seraphinite accelerator» for boost my projects
* __Team:__	1 Developers, 1 Technical Specialist
* __Participation:__	Frontend development, create sites on Elementor. Using the hook in conjunction with the ACF plugin + writing code for custom fields.
* __Tools and technologies:__	PHP 7.4 – 8.0, MySQL old version, WordPress , ElementorPro, ACF, CPT UI, php wp Hooks, JS(for security against pressing hot keys), Crocoblock Jet Widgets, seraphinite accelerator.


## June 2020 – December 2020
### Technical Specialist & Developer
* __Project:__	Setting up ready-made projects on the theme of The 7 + ElementorPro in WeSoftYou (remote work), creating projects on WordPress + Elementor, using ACF + CPT UI + Crocoblock Jet Widgets(landing pages and full-fledged sites). Using the plugin «seraphinite accelerator» for boost my projects
* __Team:__	1 Developers, 1 Technical Specialist
Participation:	Setting up on the site, with the inclusion of third-party services
* __Tools and technologies:__	PHP 7.4 – 8.0, MySQL old version, WordPress , ElementorPro, ACF, CPT UI, php wp Hooks, JS(for security against pressing hot keys), Crocoblock Jet Widgets, seraphinite accelerator, wp rocket, autoptimize, wp-optimize, w3 total cache


## March 2020 – May 2020 
### Technical Specialist
* __Project:__	Setting up payment systems for the online store WooCommerce, Nets Easy and Paypal, setting up the Shipmondo delivery system, setting up MailChimp mailing system
* __Team:__	1 Developers, 1 Technical Specialist
* __Participation:__	Setting up on the site, with the inclusion of third-party services
* __Tools and technologies:__	PHP 7.3, MySQL 5.6, WooCommerce, Nets Easy, PayPal, Shipmondo, MailChimp, WordPress.

## December 2019 – January 2020 
### Developer
* __Project:__	Website development based on WordPress. Experience in developing sites realties with using ACF plugin and custom fields.
* __Team:__	1 Developer
* __Participation:__	Using the hook in conjunction with the ACF plugin + writing code for custom fields.
* __Tools and technologies:__	PHP 7, ACF, MySQL 5.6,Custom fields, php-hooks, Brackets, WordPress 

## August 2018 – November 2019 
### Developer
* __Project:__	Website development based on WordPress. Experience in developing sites for organizations, online store on WooCommerce.
* __Team:__	1 Developer
* __Participation:__	Frontend development, setting up sites on WooCommerce, create sites on Elementor 
* __Tools and technologies:__	PHP 7, WordPress, WooCommerce, Elementor,  MySQL 5.6, HTML, CSS, Notepad++, Brackets 




## January 2017 – February 2018 
### HTML-Layout
* __Project:__	Website development based on HTML5, CSS3, WordPress, Joomla, DLE. 
* __Team:__	1 HTML-Layout (he's a developer)
* __Participation:__	Frontend development, Transferring the site template to the selected CMS 
* __Tools and technologies:__	PHP 5.6,  WordPress, Bootstrap, MySQL 5.6, HTML5, CSS3, Notepad++, Sublime Text, Joomla, Data Life Engine (DLE) 

## March 2014 – November 2015
### Developer
* __Project:__	Website development based on WordPress. Experience in developing both simple postcard sites and sites for organizations and institutions. Creating blogs for friends.
* __Team:__	1 Developers
* __Participation:__	Custom themes development
* __Tools and technologies:__	PHP 5.2.4, PHP 5.3, WordPress, MySQL 5.3,  CSS, HTML, Sublime Text, Notepad++


# Completed projects


## The projects can be found at the link below:

https://www.behance.net/c4299cb7



# Education

## 2015

__Gomel State University named after F. Skarina, Historian Faculty__ 
* __Teacher of history__

## 2017

__ITSTEP Academy__
* __Trainee/Junior Testing Engineer__

## 2020

__GeekBrains Mail.ru Group__

* __Teacher of the basics of algorithmization__