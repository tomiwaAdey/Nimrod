# Welcome to Nimrod
Nimrod is a lead generation bot that helps you find the emails of people you want to reach out to.

You hand Nimrod a google spreadsheet with the details of your prospects, and it fills in their emails from several tools for you.

A more detailed explanation of Nimrod processes and how it works can be found here:
[http://www.scrappycabin.com/blogs/the-nimrod-recipe](http://www.scrappycabin.com/blogs/the-nimrod-recipe)

In short, Nimrod turns this:
![Prospect spreadsheet](https://lh5.googleusercontent.com/I5LAxRDbAz4-CwaWKl-vQBLHsqVrqvpN8dveCfymVuDXj17hcKdnv7GaJwFyvwQJBERJpAUFgkvwnCc_UopUgyNgcSWd4I0UEAdEP3VDPaBlLRDBvVTgBbkxev0jBLv6XTqIJTQJ)

Into this:
![Completed prospect spreadsheet](https://lh4.googleusercontent.com/88kQKT5FYiqzahwBY_Bfl0i0OJKgF4YBYzQhhfKvbUUSGFqrsrHtVKsgqnvDUI91Ts40rZ0fxkOKle-Lb6NRYl7i3S09PimpWrVPTzQYKi_z2VTBjvqUZdxx9gF738qWSjSv0KyZ)

##How does Nimrod do his job?
- Nimrod starts at the spreadsheet, it signs into your google drive and opens the spreadsheet you’ve specified.
- For every prospect in your spreadsheet, it gets their name and domain.
- It visits several tools one-by-one, on your behalf, enters the name and domain in the tool and fills the spreadsheet with the email suggestion returned.
- It continues until it has exhausted all the prospects in the spreadsheet.
- It hands you a completed spreadsheet.
- It stops and it’s eager to get more work.

> Nimrod can work 24hrs a day every day, it doesn’t complain, it doesn’t make mistakes, and it doesn’t ask you for money.

Find out more about how Nimrod works here: [http://www.scrappycabin.com/blogs/the-nimrod-recipe](http://www.scrappycabin.com/blogs/the-nimrod-recipe)


## Setup for non-techies

[Follow the guide here.](http://www.scrappycabin.com/blogs/the-nimrod-recipe#a3)


## Setup

* To get started, get a list of prospects in a google spreadsheet. [Click here to get a sample template](https://docs.google.com/spreadsheets/u/2/d/1NTHbSxdr9PMKXf-wpWwaT44FR8YuLqRMPrURWwvaGC0/edit). It’s important that you do not change the format of the columns
* Clone this repo in a local folder
### If you are using mac, you will already have ruby pre-installed on your machine
* Run these commands in terminal:
```
gem install google_drive
brew install phantomjs
gem install watir-webdriver
```
* If you don't have Homebrew installed, run:
```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
### If you are using windows:
* Install Ruby with [Ruby Installer](https://rubyinstaller.org/downloads/)
* Install [DevKit](http://rubyinstaller.org/add-ons/devkit/)
* Install [phantomjs](https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-2.1.1-windows.zip)
* run `gem install watir-webdriver`
* Then run `gem install google_drive`
### Now that the setup is done,
* Navigate to the Nimrod folder and open it in your favourite code editor
* Fill in your details in `@your_config`
* The google spreadsheet keys can be found in the URL. It’s the alphanumeric keys between `d/` and  `/edit` in the URL
* Open the `gdrive_config.json` file and enter your google `client_id` & `client_secret`. [Follow this guide to get them](http://www.scrappycabin.com/guides/google-drive-authorisation/)
* You’re good to go. Run:
```
ruby Nimrod.rb &
```

## Would you like a web version of Nimrod?
It’ll look something like this:
![Prospect spreadsheet](https://lh3.googleusercontent.com/Dvyzo2Pos3q9hGHmVGvpBZNsmkfxO3EkTtrkzCF-u4J3yo6_ry1Rk_T_XkWLGqEGp1X-9SiPPgshY81jeeyYrqmfQCBqHZ1aQNN2LO8b9twzz_DEKaz-tjEC9H7_Rd6XI-rRRjRZ)

[Find out how to get it for free here.](http://www.scrappycabin.com/blogs/the-nimrod-recipe#blog-action-step)

### Report a bug & Contact

If you'd like to report a bug, or if you have any questions or feedback, get in touch via [tomiwa@scrappycabin.com](mailto:tomiwa@scrappycabin.com).
<br />
[Facebook](https://facebook.com/tomiwaAdey) [Twitter](https://twitter.com/tomiwaAdey)
