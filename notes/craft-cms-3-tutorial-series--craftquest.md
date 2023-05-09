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

composer.json (dependences)
composer.lock 
config/ (config files)
    app.php (pulls from .env)
    db.php
    general.php (set/pulled from .env)
    license.key (license key for craft)
    redactor/ (wysiwyg editor, config)
    routes.php (for rendering, templates)
craft.exec (updates...)
craft.bat (?)
migrations/ (for migrations)
modules/ (custom modules)
storage/ (for backups/logs/runtime cache)
templates/ (for templates... most used)
vendor/ (where composer, stores the packages needed)
web/ (public)

In the command line: `ls -al`

## [Craft CMS Tutorial, Part 13: Securing Craft CMS with cpTrigger](https://www.youtube.com/watch?v=EcNkS9yOkjY&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=14)

config/general.php

```
// control Panel trigger word
'cpTrigger' => 'admin',
```

After changing this the admin, url will give a 404 error.

If you got to: `website-url.domain/new-cpTrigger` it will bring up the admin area.

## [Craft CMS Tutorial, Part 14: Intro to Craft CMS Plugins](https://www.youtube.com/watch?v=hTONY9_OHY0&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=15)

Admin > Plugin Store

Allows you to extend what the Craft CMS can do. IF the default functionality doesn't meet your needs.

Install Plugins, from command line

`composer require craftcms/feed-me`

`./craft help`

`./craft install/plugin feed-me`

Dpendencies, is technical debt 

... they have videos on feed-me
... they have videos on how to create plugins (not covered in this course)

## [Craft CMS Tutorial, Part 15: What is devMode?](https://www.youtube.com/watch?v=PDU-7NxSXDo&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=16)

Bottom-Left of Admin, indicator of Dev Mode. Full Stack Error Messages. On frontend AND in storage/logs/web.log

Also Dump with Twig? And Cache disabled.

config/general.php
`'devMode' => true,`
.env (.env not shared...)
`ENVIRONMENT="dev"`

## [Craft CMS Tutorial, Part 16: Debugging with the Yii Debug Toolbar](https://www.youtube.com/watch?v=2lMSaN5wMaU&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=17)

Craft CMS, is built on Yii.

Users/Prefences/Debug Toolbar

Bottom-Right, on Frontend/Backend

... video doesn't match content ...

## [Craft CMS Tutorial, Part 17: The Pieces of Craft](https://www.youtube.com/watch?v=CL26aqEldVY&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=18)

- Sections - how we organize content or data in craft
    -   Types:
        - Channel 
            - collection of related entries
            - keep adding to over time
        - Structure
            - similar to channels
            - hierarchy/nesting, which is reflected in the URLs
                - /about
                - /about/offices
                - /about/offices/austin
        - Single
            - one-off entry
            - unique content requirements that are not shared with any other entries on the site.
- Fields & Field Types - define content types we store as entries
- Entries - how the content is stored in a Section
- Templates - used to display content to the end user (typically in the web browser via Twig)
- More....

## [Craft CMS Tutorial, Part 18: Moving the Assets to the Project](https://www.youtube.com/watch?v=2IquITmeG7Y&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=19)

Access the template code here: https://gitlab.com/craft-cms-training/crafty-coffee-templates

This is just the static template code. NOT implimented into Craft CMS...

bower_components/, images/, js/, stylesheets. copy over too the web/ directory in the craft project...

## [Craft CMS Tutorial, Part 19: Defining Craft Sections and Fieldss](https://www.youtube.com/watch?v=9z7lb_P-Sb4&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=20)

Content Chunks...
    - Drinks (channel)
        - Name
        - Category
        - BackgroundImage
        - Content/Images
        - Recipe Link
    - News (channel)
        - Name
        - Author
        - Content
    - Recipe (?)
    - About (?)
        - Name/Title
        - Subtitle
        - Content

## [Craft Tutorial Series, Part 20: Creating Sections and Fields](https://www.youtube.com/watch?v=HsMHG84znkI&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=21)

Admin/Settings/Sections/New/

name: 'name'
section type: 'channel'
Template: drinks/_entry.twig // .twig not needed.

Save

templates/drinks/_entry.twig

Entry Types...

Admin/Settings/Fields/New/

Fields can be Grouped into Groups

name: 'intro'
Handle: 'intro'

Field Type: 'Plain Text'

Redactor, install plugin...

...




## [Craft CMS Tutorial, 21: Creating Publish Layouts](https://www.youtube.com/watch?v=Nfaen5uMzKI&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=22)

Admin/Settings/Sections/'section'/entry-type

Admin/Entries

## [Craft CMS Tutorial, Part 22: Creating Single Sections (Homepage)](https://www.youtube.com/watch?v=wkUNxXyOFRo&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=23)

Admin/Settings/Sections/New

Name: Homepage

Section Type: Single

Template: index

Save

Admin/Entries/Singles

## [Craft CMS Tutorial, Part 23: Creating Asset Volumes and Transforms](https://www.youtube.com/watch?v=2ijzUn-uCho&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=24)

Images Field...

Assets

- Manage files using the Assets manager
- Like a file manager
- Only stores references to the files on disk
- Easily access them in templates

Asset Volumes

- Local - stored right on disk of server (For course)
- Remote - stored in a supported third party cloud service (AWS S3, Google Cloud, Rackspace Cloud, Digital Ocean Spaces... etc) plugins required

Admin/Settings/Assets/

Volumes, Image Transforms, Settings...

Volume/New

Name:
Public urls...
Base URL:
@web/images/uploads/drinks
Volume Type:
Local folder
File System Path:
@webroot/images/uploads/drinks

Save

Try upload on Admin/Assets

Admin/Settings/Fields/New/

name: 'image'
Handle: 'image'

Field Type: 'Assets'

Generate Thumbs for images, using Image Transforms. (Admin/Settings/Assets/)

## [Craft CMS Tutorial, Part 24: Creating Nested Pages with Structure Sections](https://www.youtube.com/watch?v=neGLf15_dnk&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=25)

For about pages...

Admin/Sections/New/

name: 
section type: structure

Entry URL:
{parent.uri}/{slug}

Template: about/_entry.twig // .twig not needed.

Save

templates/about/_entry.twig

`<h1>{{ entry.title }}</h1>`

...


## [Craft CMS Tutorial, Part 25: On Your Own Review](https://www.youtube.com/watch?v=-5aegC0uD78&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=26)

Required fields*

...

## [Craft CMS Tutorial, Part 26: Introduction to Coding Templates with Twig in Craft CMS](https://www.youtube.com/watch?v=yklu5rR67JQ&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=26)

Building Craft Templates
- Brief introduction to Twig
- Basics of Twig and Craft

- Implement homepage
- Implement Drinks detail template
- Implement News detail template
- Implement Structure template for About section

## [Craft CMS Tutorial, Part 27: Introduction to Twig](https://www.youtube.com/watch?v=PIPLraLG4rw&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=27)

Twig, is not part of 
Suggest, taking Twig Craft Course...

This course only covers the basics...


for loop

```
{% for drink in drinks %}
    {{ drink.title }}
{% endfor %}
```

## [Craft CMS Tutorial, Part 28: Learn Layouts and Blocks in Twig](https://www.youtube.com/watch?v=PPBFAqj5L3U&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=28)

index.twig

```
{% extends "_layouts/main" %}
{% block main %}
    (page content)
{% endblock %}
```

_layouts/main.twig (header)(footer)

```
(header)
    {% block main %}

    {% endblock %}
(footer)
```

## [Craft CMS Tutorial, Part 29: Coding Entry Listings Pages](https://www.youtube.com/watch?v=Sb8Ho0mGrMo&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=29)

index.twig

```
{% extends "_layouts/main" %}
{% block main %}
    (page content)
    {{ entry.subtitle }} // from field name(subtitle)

    {% for drink in craft.entries.section('drinks').limit(5).all() %}
        {{ drink.url }}
        {{ drink.drinkimage.one().url() }}
        {{ drink.title }}
    {% endfor %}

    {% for item in craft.entries.section('news').limit(10).all() %}
        {{ item.url }}
        {{ item.excerpt }}
    {% endfor %}

{% endblock %}
```

_layouts/main.twig (header)(footer)

```
(header)
    {% block main %}

    {% endblock %}
(footer)
```

Has video on seeding, fake content into a project....

## [Craft CMS Tutorial, Part 30: Coding an Entry Template](https://www.youtube.com/watch?v=B4LlkLkgovc&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=30)

drinks/_entry.twig

defined in the settings.

```
{% extends "_layouts/main" %}
{% block main %}
    (content)
    {{ entry.title }}
    {{ entry.title }}
    {{ entry.introduction }}
    {{ entry.pageCopy }}
{% endblock %}
```

## [Craft CMS Tutorial, Part 31: Reviewing Your Twig Template Work](https://www.youtube.com/watch?v=KOp8fXU3XBE&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=31)

news/_entry.twig

defined in the settings.

```
{% extends "_layouts/main" %}
{% block main %}
    (content)
    {{ entry.excerpt }}
    {{ entry.title }}
    {{ entry.author }}
    {{ entry.newsBody }}
{% endblock %}
```

## [Craft CMS Tutorial, Part 32: On Your Own - Creating a Section Listing Page](https://www.youtube.com/watch?v=7xAdPmyIJX8&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=32)

...

## [Craft CMS Tutorial, Part 33: Reviewing Your Work Coding Section Listing Templates](https://www.youtube.com/watch?v=RvgrDInUIRA&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=33)

drinks/index.twig

```
{% extends "_layouts/main" %}
{% block main %}

(content)

    {% for drink in craft.entries.section('drinks').limit(25).all() %}
        {{ drink.url }} {{ drink.title }}
    {% endfor %}

{% endblock %}
```

news/index.twig

```
{% extends "_layouts/main" %}
{% block main %}

(content)

    {% for item in craft.entries.section('news').limit(25).all() %}
        {{ item.url }} {{ item.title }}
        {{ item.author }} {{ item.postDate | date('M d, Y') }}
    {% endfor %}

{% endblock %}
```

## [Craft CMS Tutorial, Part 34: Coding a Structure Section Entry Template](https://www.youtube.com/watch?v=p2OsxEryODU&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=34)


about/_entry.twig

```
{% extends "_layouts/main" %}
{% block main %}

(content)

{{ entry.title }}
{{ entry.title }}
{{ entry.subtitle }}
{{ entry.pageIntro }}
{{ entry.pageCopy }}

{% endblock %}
```

## [Craft CMS Tutorial, Part 35: Creating a Matrix Field in Craft](https://www.youtube.com/watch?v=PwmrGTwVkQA&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=35)

Matrix Field

- Create multiple blocks of content in a single field
- Each block can contain multiple fields and field types
- Create multiple instances of the same block
- Re-order Matrix blocks to customize the content flow

Matrix field Blocks

- Recipe Image: Image field, Image caption (plain text)
- Reciple Tip: Plain text field
- Recipe Copy: Rich text field
- Reciple Steps: Steps title (plain text), Steps (table)

Admin/Settings/Sections/New/

Recipes
Channel

recipes/_entry.twig

Admin/Settings/Fields/New/

Field type: Matrix

...

## [Craft CMS Tutorial, Part 36: Coding a Matrix Field in Craft](https://www.youtube.com/watch?v=uRWfYigyXTg&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=36)

recipes/_entry.twig

```
{% extends "_layouts/main" %}
{% block main %}

        (content)

        {{ entry.title }}
        {{ entry.title }}


        {% for block in entry.recipeContents %}

        <!-- {% if block.type == 'recipeImage' %} -->

            {% switch block.type %}
                {% case 'recipeImage' %}

                    {% set image = block.image.one() %}

                    {# recipeImage Block #}

                    {{ image.url }}

                    {% if block.imageCaption %}

                        {{ block.imageCaption}}

                    {% endif %}

                    {# End recipeImage Block #}

                {% case 'recipeCopy' %}

                    {# recipeCopy Block #}

                        {{ block.bodyContent }}

                    {# End recipeCopy Block #}

                {% case 'recipeIngredients' %}

                    {# recipeIngredients Block #}

                        {% for row in block.ingredients %}
                        
                            {{ row.amount }}
                            {{ row.ingredient }}

                        {% endfor %}

                    {# End recipeIngredients Block #}

                {% case 'recipeSteps' %}

                    {{ block.stepsTitle }}

                    {# recipeSteps Block #}

                        {% for step in block.stepsContent %}
                        
                            {{ step.stepInstructions }}

                        {% endfor %}

                    {# End recipeSteps Block #}


                {% case 'recipeTip' %}

                    {# recipeTip Block #}

                        {{ block.tipContent }}

                    {# End recipeTip Block #}

            {% endswitch %}

        <!-- {% endif %} -->

        {% endfor %}

    {% endif %}

{% endblock %}
```


## [Craft CMS Tutorial, Part 37: Setting Up Categories in Craft](https://www.youtube.com/watch?v=qzjhXrmA9gc&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=37)

Admin/Settings/Categories/

Category Groups

/New

styles/_entry.twig

Field Layouts?

Create Fields...

name: Style Description
Type: Plain Text

Categories/New/

...

Create Fields... for sections.

name: Drink Style
Type: Catagories
Source: Drink Styles

Add to Recipes


## [Craft CMS Tutorial, Part 38: Coding a Category Listing](https://www.youtube.com/watch?v=5ckzvffXkOY&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=38)

styles/_entry.twig

Listing of all the entires of a category

```
{% extends "_layouts/main" %}
{% block main %}

    (content)

    {{ category.title }}

    {{ category.title }}

    {{ category.styleDescription }}

    {# Drinks Entries #}
        {% for drink in craft.entries.section('drinks').relatedTo(category).all() %}
            {{ drink.url }} {{ drink.title }}
            {{ drink.entryDate | date('M Y') }}
        {% endfor %}
    {# End Drinks Entries #}

    {# Recipes Entries #}
        {% for recipe in craft.entries.section('recipes').relatedTo(category).all() %}
            {{ recipe.url }} {{ recipe.title }}
            {{ recipe.entryDate | date('M Y') }}
        {% endfor %}
    {# End Recipes Entries #}

{% endblock %}
```

## [Craft CMS Tutorial, Part 39: Coding a Category Index](https://www.youtube.com/watch?v=NssfLDlhM8w&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=39)

drinks/index.twig

```
{% extends "_layouts/main" %}
{% block main %}

(content)

    {% for drink in craft.entries.section('drinks').limit(25).all() %}
        
        {{ drink.url }} {{ drink.title }}

        {% set style = drink.drinkStyle.one() %}

        {{ style.url }} {{ style.title}}

    {% endfor %}

{% endblock %}
```

styles/index.twig

```
{% extends "_layouts/main" %}
{% block main %}

(content)

    {% set styles = craft.categories.group('drinkStyles').all() %}

    {% for style in styles %}
        {{ style.url }} {{ style.title }}
        {{ style.styleDescription }}
    {% endfor %}

{% endblock %}

```

## [Craft CMS Tutorial, Part 40: Relating Entries with the Entries Field](https://www.youtube.com/watch?v=rnl23P_xP0I&list=PLCy7dPypkr2rOlj9Ps5HbzYeJecL48yg-&index=40)

Settings/Fields/

Drinks/New

name: Drinks Recipe
type: Entries

Source: Recipes

...

drinks/_entry.twig

```

{% set drinkRecipe = entry.drinkRecipe.one() %}
{{ drinkRecipe.url}} {{ entry.title }}

```

... duplicates???
