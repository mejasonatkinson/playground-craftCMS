# [Craft CMS 3 Tutorial Series; CraftQuest](https://www.youtube.com/playlist?list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-)

## [Craft CMS Tutorial, Part 1: Introduction](https://www.youtube.com/watch?v=x5bVKZxFdPo&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=1)

Craft CMS was created by [Pixel & Tonic](https://pixelandtonic.com/)

- Yii framework
- PHP/MySQL foundation but can also use postgresql
- Twig Templating language

## [Craft CMS Tutorial, Part 2: What We'll Learn in this Course About Craft CMS](https://www.youtube.com/watch?v=9i5QSLgXvqE&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=2)

What We'll Learn

- [ ] How to install and configure Craft
- [ ] Become familiar with Craft Control Panel, files & directories
- [ ] Convert static HTML to Craft templates using Twig
- [ ] Plan and create content Sections, Fields, Field Layouts
- [ ] Create Asset sources, generate thumbnails authomatically
- [ ] Learn basics of Twig templating, template inheritance
- [ ] Assign and display Categories
- [ ] Set up and use the powerful Matrix field

## [Craft CMS Tutorial, Part 3: What We're Building with Craft CMS](https://www.youtube.com/watch?v=a1WR-ZvRoOs&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=3)

Project: Crafty Coffee

## [Craft CMS Tutorial, Part 4: Server Requirements for Craft CMS](https://www.youtube.com/watch?v=GKeyXg3nhjk&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=4)

**Requirements**

- PHP 7.0 or later
- MySQL or later with InnoDB
- PostgreSQL 9.5+
- A web server (I use Apache)
- At least 256 MB memory allocated to PHP

**PHP Requirements**

- PCRE
- PDO
- GD or ImageMagick
- OpenSSL
- MultibyteString
- JSON
- cURL
- Reflection
- SPL
- Zip

**Database Requirements**

- MySQL and PostgreSQL
- Database credentials (including database name)
- Database user should have read/write permissions

**Permissions**

- craft/config
- craft/storage

## [Craft CMS Tutorial, Part 5: Craft CMS Licensing Options](https://www.youtube.com/watch?v=a7QqZtS6bic&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=5)

[Craft CMS Pricing](https://craftcms.com/pricing)

- Solo - Free
- Pro (Free Local)
- Enterprise (on request)

## [Craft CMS Tutorial, Part 6: What is Composer? (Craft CMS)](https://www.youtube.com/watch?v=TNojJL_rAxY&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=6)

- A Dependency manager that handles all of the software needed to run an app or project
- You tell Composer what your project needs to run
- Composer will install those dependencies for you
- Composer handles dependencies for a project, it does not install packages globally
- It helps you to keep your dependencies separate from your project code
- It defines your project dependencies in a composer.json file

...

## [Craft CMS Tutorial, Part 7: Installing Composer](https://www.youtube.com/watch?v=77ZSHSIa_wA&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=7)

**Tutorial being run on a Mac**

Follow the instructions on [getcomposer.org](https://getcomposer.org/) to complete installation.

## [Craft CMS Tutorial, Part 8: Installing Craft with Composer](https://www.youtube.com/watch?v=iC9DN0c8NQc&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=8)

Could not proceed locally, ran into a issue with **PHP's intl extension** 

Due to this I will not be going any further with this tutorial.

...


## [Craft CMS Tutorial, Part 9: Running the Craft CMS Setup Wizard from the Browser](https://www.youtube.com/watch?v=sq-q9WENKog&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=10)

Need to access it locally, first via:
- mamp...
- xamp,,,
- valet...
- etc

`ls -al`

Looking for .env file...

Check to make sure this is complete...

Go to localhost... and you can install craft... (this can also be done in the commandline)

Upgrade Craft CMS... Try Pro... To get access to all features. This is fine for local development but when deployed you will need to buy a license.

## [Craft CMS Tutorial, Part 10: What is env? (Craft CMS)](https://www.youtube.com/watch?v=VliMbA8SJq8&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=11)

New to craft 3.

- Where you store environment-specific settings
- E.g. Database connection information
- Uses PHPDotEnv (based on Ruby's dotenv)

- You have a .env file in your project root
- Using keys and values, you set environment variables.
- Anything you set is accessible globally via the `$_ENV` global, which you can retrieve via `getenv('key')`.
- Use your .gitignore file to ignore this file so it is not tracked in your repository.
- PHPDotEnv is a dependency for Craft CMS

`vim .env` to see how all the values are stored.

`cd config/`

`ls`

`vim db.php` If you look at the return you will see how these env values are retrieved using `getenv('key')`.

## [Craft CMS Tutorial, Part 11: Touring the Craft CMS Control Panel](https://www.youtube.com/watch?v=6qvu0SkDq_E&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=12)

`/admin`, Login...

- Dashboard
    - New widgets (if wanted..), Also ability to create new widgets, if your coding level allows
- Users
- GraphQL (only for pro)
- Utilities
    - For application info...
    - Database backup...
- Settings (if admin user) <------ where most of the content in this course focuses on.
- Plugin Store

## [Craft CMS Tutorial, Part 12: Touring the Craft CMS Files and Directories](https://www.youtube.com/watch?v=4oQaddQJjVY&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=14)

## [Craft CMS Tutorial, Part 13: Securing Craft CMS with cpTrigger](https://www.youtube.com/watch?v=EcNkS9yOkjY&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=14)

## [Craft CMS Tutorial, Part 14: Intro to Craft CMS Plugins](https://www.youtube.com/watch?v=hTONY9_OHY0&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=15)

## [Craft CMS Tutorial, Part 15: What is devMode?](https://www.youtube.com/watch?v=PDU-7NxSXDo&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=16)

## [Craft CMS Tutorial, Part 16: Debugging with the Yii Debug Toolbar](https://www.youtube.com/watch?v=2lMSaN5wMaU&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=17)

## [Craft CMS Tutorial, Part 17: The Pieces of Craft](https://www.youtube.com/watch?v=CL26aqEldVY&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=18)

## [Craft CMS Tutorial, Part 18: Moving the Assets to the Project](https://www.youtube.com/watch?v=2IquITmeG7Y&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=19)

## [Craft CMS Tutorial, Part 19: Defining Craft Sections and Fieldss](https://www.youtube.com/watch?v=9z7lb_P-Sb4&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=20)

## [Craft Tutorial Series, Part 20: Creating Sections and Fields](https://www.youtube.com/watch?v=HsMHG84znkI&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=21)

## [Craft CMS Tutorial, 21: Creating Publish Layouts](https://www.youtube.com/watch?v=Nfaen5uMzKI&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=22)

## [Craft CMS Tutorial, Part 22: Creating Single Sections (Homepage)](https://www.youtube.com/watch?v=wkUNxXyOFRo&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=23)

## [Craft CMS Tutorial, Part 23: Creating Asset Volumes and Transforms](https://www.youtube.com/watch?v=2ijzUn-uCho&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=24)

## [Craft CMS Tutorial, Part 24: Creating Nested Pages with Structure Sections](https://www.youtube.com/watch?v=neGLf15_dnk&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=25)

## [Craft CMS Tutorial, Part 25: On Your Own Review](https://www.youtube.com/watch?v=-5aegC0uD78&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=26)

## []()

## []()

## []()

