# Welcome to Nimrod
Nimrod is a lead generation bot that helps you find the emails of people you want to reach out to.

You hand Nimrod a google spreadsheet with the details of your prospects, and it fills in their emails from several tools for you.

## Setup

* To get started, get a list of prospect in a google spreadsheet. [Click here to get a sample template](https://docs.google.com/spreadsheets/u/2/d/1NTHbSxdr9PMKXf-wpWwaT44FR8YuLqRMPrURWwvaGC0/edit). It’s important that you do not change the format of the columns
* Install Ruby
* Clone this repo in a local folder
* Run these commands in terminal:
```
gem install google_drive
gem install watir-webdriver
```
* Navigate to the Nimrod folder and open it in your favourite code editor
* Fill in your details in `@your_config`
* The keys the google spreadsheet can be found in the URL. It’s the alphanumeric keys between `d/` and  `/edit` in the URL
* Open `google_drive_config.json` file and enter your google `client_id` & `client_secret`. [Follow this guide to get them](http://www.scrappycabin.com/guides/google-drive-authorisation/)
* You’re good to go. Run:
```
ruby Nimrod.rb
```
