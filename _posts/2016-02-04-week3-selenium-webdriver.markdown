---
layout: post
title:  Week 3 - Selenium Webdriver 
date:   2016-02-04 20:36:09
categories: makers blog ronin
tags: [makers]
---

![Selenium Element](/images/selenium.png)

Also known as element 34, to Ruby developers it is better known as an automation tool to visually test Capybara commands in your unit and feature tests directly in the browser.

Whilst pairing earlier this week, my partner and I managed to figure out a way to get our feature test to run directly in the browser. Having previously completed the Capybara tutorial challenge ealier in the morning, we realised that the same commands we had spiked in Pry in order to send clicks to the webpage could be of use. 

First we had to require the correct gems in our feature test spec:

{% highlight ruby %}
require 'capybara/dsl'
require 'selenium-webdriver'
{% endhighlight %}

If any of the requires failed, then it was simply a matter of updating the Gemfile for bundle to install the gems and dependencies. Then in our scenario test blocks, add the following:

{% highlight ruby %}
before do
    include Capybara::DSL
    Capybara.default_driver = :selenium
end
{% endhighlight %}

What will now happen is that when you run your rspec tests, Selenium will open a browser (Firefox in my case) and as if by 'magic' start clicking buttons or filling in input forms - basically whatever you've written in your tests either until the test passes or produces an error.

A few of my peers have found this especially useful in seeing a visual representation of their tests running, and helpful in that it can aid in the debugging process, where the alternative is just a Ruby error stack trace or RSpec failure in the command line. The code can be further refactored into a method within the same spec file, or as a web_helper method in a seperate spec file, and call it as you need it.



