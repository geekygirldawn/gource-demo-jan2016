# Visualize your repos: Navigate the myriad of Gource configuration options

Various Gource configuration options and how to tweak them to make Gource work
better for your repo.

## Presentation Logistics

* [FLOSS Community Metrics Meeting](http://flosscommunitymetrics.org/) 
* Open Source Software Development Analytics Conference
* January 29, 2016 - Brussels (before FOSDEM)
* 17:05 - 17:10: A 5 minute Lightning Talk

## Getting Started

[Install Gource](http://gource.io/) and run it on your repo with the default options

    gource /path/to/your/repo

## Demo

**Small Repository with Light Activity**

    gource --logo images/bitergia_logo_sm.png --title "MailingListStats AKA mlstats" --key --start-date '2014-01-01' --user-image-dir images -a 1 -s .05 --path ../MailingListStats

## Gource Configuration Options

**Repo:**

* --path /path/to/repo (or omit and run Gource from the top level of the repo dir)

**Display options:**

* --logo images/bitergia_logo_sm.png 
* --title "MailingListStats AKA mlstats" 
* --key (shows color key for file types)
* --start-date '2014-05-01'
* --user-image-dir images (Directory with .jpg or .png images of users 'Full Name.png' for avatars

**Speed up repos with less activity:**

* -a 1 (auto skip to next entry if nothing happens in x seconds - default 3)
* -s .05 (speed in seconds per say - default 10

**While Gource is running:**

* Space bar to pause
* <Ctrl> + / - to speed up or slow down
* Use arrow keys to move camera
* Mouse over timeline widget at the bottom and click on a date to move in time.

## More Info about Gource

More info about [Gource](http://gource.io/),
including downloads and information about installation. You can
also look at the presentation I did about Gource at the
[FLOSS Community Metrics Meeting](http://www.slideshare.net/geekygirldawn/floss-community-metrics-gource-custom-log-formats) on using the Gource [custom log format](https://github.com/acaudwell/Gource/wiki/Custom-Log-Format)
option. 

I recommend playing around with the different controls to speed things up / slow down or show / hide
things to get something that looks good with your data. Most of this information can be found
using gource -H, but the [control page](https://github.com/acaudwell/Gource/wiki/Controls)
on the wiki and the [Gource README](https://github.com/acaudwell/Gource) has more details about the controls. 
You might also check out these [templates]
(https://github.com/FOSSRIT/gourciferous/tree/develop/Templates) with recommended configurations
for different types of data (large projects, long-lived projects, etc.)

You can also check out [Gourciferous](https://github.com/FOSSRIT/gourciferous) for visualizing multiple
repos in a single visualization using the custom log format.
