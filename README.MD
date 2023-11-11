# Achron Wiki Rough-Scrape Repo
Hi!

So it seems the Achron wiki has not updated its security certificate for a long time, now!

This repo is not the full site; it's missing all of its editable wiki functionality, search functions, and a few pages here and there.
However, the goal was to get the vast majority of data downloaded and available offline, until the certs are updated!

People are free to tweak and update this, if they have ideas for fixing stuff.

This is more-or-less what I used to scrape the site:
```
curl -o "./backup/Page_Name.html" -k --tls-max 1.1 --ciphers DEFAULT@SECLEVEL=0 'https://www.achrongame.com/wiki/index.php?Page_Name'
```

I had to do a ***lot*** of custom replacements, rearrangements, and add a dark mode theme, just to get all the references to work.
The wiki did not want to export using the *intended* tools, likely due to the cert problem.

What a day I spent! Whew!

(**Full disclosure:** I am not the original dev of Achron; I'm just a fan.)