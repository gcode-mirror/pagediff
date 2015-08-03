# Goals #

The goal of pagediff is to provide users a tool to monitor pages and send alerts when a change is spotted.
Alerts are sent by emails or shown in rss feeds, and archives of the last _n_ changes of the pages are kept for future reference.

# Details #
How will it works ?

## 3 kind of users ##
  * admin : owns the website
  * user : identified (=has an account), can CRUD his alerts
  * visitor : can create a new account

## 3 distinct applications ##
  * frontend : where the user interact with the website, all pages are secured and requires credentials (except those needed to create a new account)
  * monitor : crawl and archive pages, send alerts. Not accessible through the browser
  * backend : secured, used to manage the project (users, stats, ...)