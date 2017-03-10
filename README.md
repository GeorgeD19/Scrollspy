# Scrollspy

## What is it?

Scrollspy is something that I needed to include in a project that does not use bootstrap.
I still needed the scrollspy functionality that is bundled with bootstrap and after playing around with some alternatives, I found that the best solution was to create my own.
The idea was to create a simple solution that did pretty much everything that bootstraps solution offers.
So this is why I created this plugin.

For those that are not familiar with bootstraps scrollspy, basically this allows you to attach the plugin to a **ul** styled menu on a single page application. When you scroll down the page, the **pages** that you pass through would then mark the **li** children of your menu with an active class.

## Requirements

jQuery

## Demo

I have created a demo which you can find here:
http://codepen.io/r3plica/pen/NqbarV

## Installation

unzip the contents to your desired location and include either library on your page.

## How to use

It's really easy to use, simply initialise the script like this:

```
    $("#nav").scrollspy();
```

To pass options to the plugin, simply pass an object to the call like so:

```
    $("#nav").scrollspy({ offset: -25 });
```

## Options
Scrollspy.js can accept an options object to alter the way it behaves. These are the supported settings:

 * __activeClass__: The active class that gets added to the **li** element of the menu. Default is `active`
 * __animate__: If `true` will animate the scroll when a link is clicked. Default is `false`
 * __offset__: Adds an offset to when the link becomes active. Default is `0`
 * __onChange__: A callback triggered when the document scrolls into a new **target**
 * __onExit__: A callback triggered when the document scrolls on to a an element that is not a **target**
 * __duration__: Duration of the scroll animation when a link is clicked, default is `1000`
