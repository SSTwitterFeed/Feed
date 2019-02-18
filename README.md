# SS Twitter Feed plugin for Craft CMS 3.x

Show Recent tweets timeline on websites.

![Screenshot](resources/img/plugin-logo.png)

## Requirements

This plugin requires Craft CMS 3.0.0-beta.23 or later.

## Installation

To install the plugin, follow these instructions.

1. Open your terminal and go to your Craft project:

        cd /path/to/project

2. Then tell Composer to load the plugin:

        composer require ssplugin/ss-twitter-feed

3. In the Control Panel, go to Settings → Plugins and click the “Install” button for SS Twitter Feed.

## SS Twitter Feed Overview

-A plugin for Craft CMS that allows you to retrieve your Twitter timeline.
You can add multiple Twitter feeds into single page using shortcodes.-

## Configuring SS Twitter Feed

-Once you’ve installed the SS-Twitter-Feed plugin. 
Go to plugin settings to connect to twitter.
Just click on button get your Twitter Access Token and Twitter Secret.-

## Using SS Twitter Feed

-You can directly access multidimensional array of your Twitter posts using following method.
Each post has Following components you can get to:

:one: **name** ( the name of the Twitter account )
:two: **screen_name** ( the screen name of the Twitter account )
:three: **text** ( Twitter text )
:four: **profile_image_url**( Profile picture of your Twitter )
:five: **url** ( the Twitter url )
:six: **image_url** ( Twitter media image url )
:seven: **retweet_count**  (Total number of retweet count  )
:eight: **favorite_count** (Total number of likes the post recieved )
:nine: **created_at**     ( The tweet post time )
:ten: **retweet_link** (The retweet link on site )
:eleven: **favorite_link** (  favorite link )

Example:
```
	{% for tweet in craft.ssTwitterFeed.displayPost() %}
    	{{ tweet.url }}
    	{{ tweet.screen_name }}
    	{{ tweet.text }}
    	{{ tweet.created_at }}
    	{{ tweet.retweet_count }}
    	{{ tweet.favorite_count }}
	{% endfor %}
```
## SS Twitter Feed Roadmap

**BENEFITS:**

:one: Hassle-free and Simple setup( No need to create Twitter App).
:two: Number of tweets to show.
:three: Increment social commitment among you and your clients.
:four: Show your Twitter content your way to perfectly match your website style.
:five: The Plugib is updated consistently with new features, bug-fixes and Twitter API changes.
:six: Support is speedy, effective and powerful.

* Release it

Brought to you by [SystemSeeders](http://www.systemseeders.com/)
