This project isn't activly maintained anymore.
If you're looking for a more advanced and up to date library, please have a look at the php-ga project from Thomas Bachem: http://code.google.com/p/php-ga



Server Side Google Analytics (SSGA) is a simple PHP 5 class, which allows to track server-side events and data within Google Analytics.

## Requirements ##
  * PHP 5.2 or up
  * Zend Framework (only for the http client; can be replaced by curl)

## Usage ##

Download and include the class in your source files.

Create a new instance of the class<br>
<b>$ga = new Elements_Tools_Serversideanalytics();</b>

Set your Google Analytics key<br>
<b>$ga->setAccountId("UA-1234567-8");</b>

Set your charset<br>
<b>$ga->setCharset("UTF-8");</b>

Set your hostname<br>
<b>$ga->setHostName("www.example.com");</b>

Set page title<br>
<b>$ga->setPageTitle("Test");</b>

Set language<br>
<b>$ga->setLanguage("de");</b>

Set a pageview<br>
<b>$ga->setPageView("/de/serverside/test");</b>

Set an event (based on <a href='http://code.google.com/apis/analytics/docs/tracking/eventTrackerGuide.html'>http://code.google.com/apis/analytics/docs/tracking/eventTrackerGuide.html</a>) <br>
<b>$ga->setEvent("Category", "Action", "Label", "Value");</b>

Submit an event<br>
<b>$ga->createEvent();</b>