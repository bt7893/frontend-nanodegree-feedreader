# Project Overview

In this project I was given a web-based application that reads RSS feeds. The original developer of this application clearly saw the value in testing, they've already included [Jasmine](http://jasmine.github.io/) and even started writing their first test suite! Unfortunately, they decided to move on to start their own company and I am now left with an application with an incomplete test suite. That's where I come in.

# Steps Performed to Prepare the Test Project
1. Downloaded the [required project assets](http://github.com/udacity/frontend-nanodegree-feedreader).
2. Reviewed the functionality of the application within my browser.
3. Explored the application's HTML (*./index.html*), CSS (*./css/style.css*) and JavaScript (*./js/app.js*) to gain an understanding of how it works.
4. Explored the Jasmine spec file in *./jasmine/spec/feedreader.js*
5. Edited the allFeeds variable in *./js/app.js* to make the provided test fail and see how Jasmine visualizes this failure in my application.

# Steps Performed to Return All Feeds to Passing State
1. Returned the allFeeds variable to a passing state.
2. Wrote a test that loops through each feed in the allFeeds object and ensured it has a URL defined and that the URL is not empty.
3. Wrote a test that loops through each feed in the allFeeds object and ensured it has a name defined and that the name is not empty.
4. Wrote a new test suite named "The menu".
5. Wrote a test that ensures the menu element is hidden by default. Analyzed the HTML and the CSS to determine how we're performing the hiding/showing of the menu element.
6. Wrote a test that ensures the menu changes visibility when the menu icon is clicked. This test have two expectations: checks the menu display when clicked and also checks if it hides when clicked again.
7. Wrote a test that ensures when the loadFeed function is called and completes its work, there is at least a single .entry element within the .feed container. Note: loadFeed() is asynchronous so this test required the use of Jasmine's beforeEach and asynchronous done() function.
8. Wrote a test that ensures when a new feed is loaded by the loadFeed function that the content actually changes. loadFeed() is asynchronous.
9. When completed - all of my tests passed.

# Jasmine References:
1. http://jasmine.github.io/
2. https://github.com/jasmine/jasmine
3. http://www.htmlgoodies.com/beyond/javascript/testing-javascript-using-the-jasmine-framework.html
4. http://code.tutsplus.com/tutorials/testing-your-javascript-with-jasmine--net-21229
