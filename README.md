## Hi there 👋


GitHub Readme Stats

GitHub Readme Stats
Get dynamically generated GitHub stats on your READMEs!

Tests Passing GitHub Contributors Tests Coverage Issues GitHub pull requests OpenSSF Scorecard



View Demo · Report Bug · Request Feature · FAQ · Ask Question

Français · 简体中文 · Español · Deutsch · 日本語 · Português Brasileiro · Italiano · 한국어 · Nederlands · नेपाली · Türkçe

Please note that documentation translations may be outdated; try to use English documentation if possible.

Love the project? Please consider donating to help it improve!

Give india logo
Are you considering supporting the project by donating to me? Please DO NOT!!!

Picture of Coromandel Express train tragedy

India has recently suffered one of the most devastating train accidents, and your help will be immensely valuable for the people who were affected by this tragedy.

Please visit this link and make a small donation to help the people in need. A small donation goes a long way. ❤️

Features
GitHub Stats Card
Hiding individual stats
Showing additional individual stats
Showing icons
Themes
Customization
GitHub Extra Pins
Usage
Demo
GitHub Gist Pins
Usage
Demo
Top Languages Card
Usage
Language stats algorithm
Exclude individual repositories
Hide individual languages
Show more languages
Compact Language Card Layout
Donut Chart Language Card Layout
Donut Vertical Chart Language Card Layout
Pie Chart Language Card Layout
Hide Progress Bars
Demo
WakaTime Stats Card
Demo
All Demos
Quick Tip (Align The Cards)
Deploy on your own
On Vercel
📽️ Check Out Step By Step Video Tutorial By @codeSTACKr
On other platforms
Disable rate limit protections
Keep your fork up to date
💖 Support the project
Important Notices
Important

Since the GitHub API only allows 5k requests per hour per user account, the public Vercel instance hosted on https://github-readme-stats.vercel.app/api could possibly hit the rate limiter (see #1471). We use caching to prevent this from happening (see https://github.com/anuraghazra/github-readme-stats#common-options). You can turn off these rate limit protections by deploying your own Vercel instance.

Uptime Badge

Important

We're a small team, and to prioritize, we rely on upvotes 👍. We use the Top Issues dashboard for tracking community demand (see #1935). Do not hesitate to upvote the issues and pull requests you are interested in. We will work on the most upvoted first.

GitHub Stats Card
Copy and paste this into your markdown, and that's it. Simple!

Change the ?username= value to your GitHub username.

[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)
Warning

By default, the stats card only shows statistics like stars, commits, and pull requests from public repositories. To show private statistics on the stats card, you should deploy your own instance using your own GitHub API token.

Note

Available ranks are S (top 1%), A+ (12.5%), A (25%), A- (37.5%), B+ (50%), B (62.5%), B- (75%), C+ (87.5%) and C (everyone). This ranking scheme is based on the Japanese academic grading system. The global percentile is calculated as a weighted sum of percentiles for each statistic (number of commits, pull requests, reviews, issues, stars, and followers), based on the cumulative distribution function of the exponential and the log-normal distributions. The implementation can be investigated at src/calculateRank.js. The circle around the rank shows 100 minus the global percentile.

Hiding individual stats
You can pass a query parameter &hide= to hide any specific stats with comma-separated values.

Options: &hide=stars,commits,prs,issues,contribs

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra&hide=contribs,prs)
Showing additional individual stats
You can pass a query parameter &show= to show any specific additional stats with comma-separated values.

Options: &show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage)
Showing icons
To enable icons, you can pass &show_icons=true in the query param, like so:

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true)
Themes
With inbuilt themes, you can customize the look of the card without doing any manual customization.

Use &theme=THEME_NAME parameter like so :

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true&theme=radical)
All inbuilt themes
GitHub Readme Stats comes with several built-in themes (e.g. dark, radical, merko, gruvbox, tokyonight, onedark, cobalt, synthwave, highcontrast, dracula).

GitHub Readme Stats Themes

You can look at a preview for all available themes or checkout the theme config file. Please note that we paused the addition of new themes to decrease maintenance efforts; all pull requests related to new themes will be closed.

Responsive Card Theme
Anurag's GitHub stats-Dark

Since GitHub will re-upload the cards and serve them from their CDN, we can not infer the browser/GitHub theme on the server side. There are, however, four methods you can use to create dynamics themes on the client side.

Use the transparent theme
We have included a transparent theme that has a transparent background. This theme is optimized to look good on GitHub's dark and light default themes. You can enable this theme using the &theme=transparent parameter like so:

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true&theme=transparent)
👀 Show example
Add transparent alpha channel to a themes bg_color
You can use the bg_color parameter to make any of the available themes transparent. This is done by setting the bg_color to a color with a transparent alpha channel (i.e. bg_color=00000000):

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true&bg_color=00000000)
👀 Show example
Use GitHub's theme context tag
You can use GitHub's theme context tags to switch the theme based on the user GitHub theme automatically. This is done by appending #gh-dark-mode-only or #gh-light-mode-only to the end of an image URL. This tag will define whether the image specified in the markdown is only shown to viewers using a light or a dark GitHub theme:

[![Anurag's GitHub stats-Dark](https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true&theme=dark#gh-dark-mode-only)](https://github.com/anuraghazra/github-readme-stats#gh-dark-mode-only)
[![Anurag's GitHub stats-Light](https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true&theme=default#gh-light-mode-only)](https://github.com/anuraghazra/github-readme-stats#gh-light-mode-only)
👀 Show example
Use GitHub's new media feature
You can use GitHub's new media feature in HTML to specify whether to display images for light or dark themes. This is done using the HTML <picture> element in combination with the prefers-color-scheme media feature.

<picture>
  <source
    srcset="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true&theme=dark"
    media="(prefers-color-scheme: dark)"
  />
  <source
    srcset="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true"
    media="(prefers-color-scheme: light), (prefers-color-scheme: no-preference)"
  />
  <img src="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true" />
</picture>
👀 Show example
Customization
You can customize the appearance of all your cards however you wish with URL parameters.

Common Options
Name	Description	Type	Default value
title_color	Card's title color.	string (hex color)	2f80ed
text_color	Body text color.	string (hex color)	434d58
icon_color	Icons color if available.	string (hex color)	4c71f2
border_color	Card's border color. Does not apply when hide_border is enabled.	string (hex color)	e4e2e2
bg_color	Card's background color.	string (hex color or a gradient in the form of angle,start,end)	fffefe
hide_border	Hides the card's border.	boolean	false
theme	Name of the theme, choose from all available themes.	enum	default
cache_seconds	Sets the cache header manually (min: 21600, max: 86400).	integer	21600
locale	Sets the language in the card, you can check full list of available locales here.	enum	en
border_radius	Corner rounding on the card.	number	4.5
Warning

We use caching to decrease the load on our servers (see #1471 (comment)). Our cards have a default cache of 6 hours (21600 seconds). Also, note that the cache is clamped to a minimum of 6 hours and a maximum of 24 hours. If you want the data on your statistics card to be updated more often you can deploy your own instance and set environment variable CACHE_SECONDS to a value of your choosing.

Gradient in bg_color
You can provide multiple comma-separated values in the bg_color option to render a gradient with the following format:

&bg_color=DEG,COLOR1,COLOR2,COLOR3...COLOR10
Available locales
Here is a list of all available locales:

Code	Locale
cn	Chinese
zh-tw	Chinese (Taiwan)
ar	Arabic
cs	Czech
de	German
en	English
bn	Bengali
es	Spanish
fr	French
hu	Hungarian
Code	Locale
it	Italian
ja	Japanese
kr	Korean
nl	Dutch
pt-pt	Portuguese (Portugal)
pt-br	Portuguese (Brazil)
np	Nepali
el	Greek
ru	Russian
uk-ua	Ukrainian
Code	Locale
id	Indonesian
ml	Malayalam
my	Burmese
sk	Slovak
tr	Turkish
pl	Polish
uz	Uzbek
vi	Vietnamese
se	Swedish
If we don't support your language, please consider contributing! You can find more information about how to do it in our contributing guidelines.

Stats Card Exclusive Options
Name	Description	Type	Default value
hide	Hides the specified items from stats.	string (comma-separated values)	null
hide_title	Hides the title of your stats card.	boolean	false
card_width	Sets the card's width manually.	number	500px  (approx.)
hide_rank	Hides the rank and automatically resizes the card width.	boolean	false
rank_icon	Shows alternative rank icon (i.e. github, percentile or default).	enum	default
show_icons	Shows icons near all stats.	boolean	false
include_all_commits	Count total commits instead of just the current year commits.	boolean	false
line_height	Sets the line height between text.	integer	25
exclude_repo	Excludes specified repositories.	string (comma-separated values)	null
custom_title	Sets a custom title for the card.	string	<username> GitHub Stats
text_bold	Uses bold text.	boolean	true
disable_animations	Disables all animations in the card.	boolean	false
ring_color	Color of the rank circle.	string (hex color)	2f80ed
number_format	Switches between two available formats for displaying the card values short (i.e. 6.6k) and long (i.e. 6626).	enum	short
show	Shows additional items on stats card (i.e. reviews, discussions_started, discussions_answered, prs_merged or prs_merged_percentage).	string (comma-separated values)	null
Note

When hide_rank=true, the minimum card width is 270 px + the title length and padding.

Repo Card Exclusive Options
Name	Description	Type	Default value
show_owner	Shows the repo's owner name.	boolean	false
description_lines_count	Manually set the number of lines for the description. Specified value will be clamped between 1 and 3. If this parameter is not specified, the number of lines will be automatically adjusted according to the actual length of the description.	number	null
Gist Card Exclusive Options
Name	Description	Type	Default value
show_owner	Shows the gist's owner name.	boolean	false
Language Card Exclusive Options
Name	Description	Type	Default value
hide	Hides the specified languages from card.	string (comma-separated values)	null
hide_title	Hides the title of your card.	boolean	false
layout	Switches between five available layouts normal & compact & donut & donut-vertical & pie.	enum	normal
card_width	Sets the card's width manually.	number	300
langs_count	Shows more languages on the card, between 1-20.	integer	5 for normal and donut, 6 for other layouts
exclude_repo	Excludes specified repositories.	string (comma-separated values)	null
custom_title	Sets a custom title for the card.	string	Most Used Languages
disable_animations	Disables all animations in the card.	boolean	false
hide_progress	Uses the compact layout option, hides percentages, and removes the bars.	boolean	false
size_weight	Configures language stats algorithm (see Language stats algorithm).	integer	1
count_weight	Configures language stats algorithm (see Language stats algorithm).	integer	0
Warning

Language names should be URI-escaped, as specified in Percent Encoding (i.e: c++ should become c%2B%2B, jupyter notebook should become jupyter%20notebook, etc.) You can use urlencoder.org to help you do this automatically.

WakaTime Card Exclusive Options
Name	Description	Type	Default value
hide	Hides the languages specified from the card.	string (comma-separated values)	null
hide_title	Hides the title of your card.	boolean	false
line_height	Sets the line height between text.	integer	25
hide_progress	Hides the progress bar and percentage.	boolean	false
custom_title	Sets a custom title for the card.	string	WakaTime Stats
layout	Switches between two available layouts default & compact.	enum	default
langs_count	Limits the number of languages on the card, defaults to all reported languages.	integer	null
api_domain	Sets a custom API domain for the card, e.g. to use services like Hakatime or Wakapi	string	wakatime.com
display_format	Sets the WakaTime stats display format. Choose time to display time-based stats or percent to show percentages.	enum	time
disable_animations	Disables all animations in the card.	boolean	false
GitHub Extra Pins
GitHub extra pins allow you to pin more than 6 repositories in your profile using a GitHub readme profile.

Yay! You are no longer limited to 6 pinned repositories.

Usage
Copy-paste this code into your readme and change the links.

Endpoint: api/pin?username=anuraghazra&repo=github-readme-stats

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra&repo=github-readme-stats)](https://github.com/anuraghazra/github-readme-stats)
Demo
Readme Card

Use show_owner query option to include the repo's owner username

Readme Card

GitHub Gist Pins
GitHub gist pins allow you to pin gists in your GitHub profile using a GitHub readme profile.

Usage
Copy-paste this code into your readme and change the links.

Endpoint: api/gist?id=bbfce31e0217a3689c8d961a356cb10d

[![Gist Card](https://github-readme-stats.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d)](https://gist.github.com/Yizack/bbfce31e0217a3689c8d961a356cb10d/)
Demo
Gist Card

Use show_owner query option to include the gist's owner username

Gist Card

Top Languages Card
The top languages card shows a GitHub user's most frequently used languages.

Warning

By default, the language card shows language results only from public repositories. To include languages used in private repositories, you should deploy your own instance using your own GitHub API token.

Note

Top Languages does not indicate the user's skill level or anything like that; it's a GitHub metric to determine which languages have the most code on GitHub. It is a new feature of github-readme-stats.

Warning

This card shows language usage only inside your own non-forked repositories, not depending on who the author of the commits is. It does not include your contributions into another users/organizations repositories. Currently there are no way to get this data from GitHub API. If you want this behavior to be improved you can support this feature request created by @rickstaa inside GitHub Community.

Warning

Currently this card shows data only about first 100 repositories. This is because GitHub API limitations which cause downtimes of public instances (see #1471). In future this behavior will be improved by releasing GitHub action or providing environment variables for user's own instances.

Usage
Copy-paste this code into your readme and change the links.

Endpoint: api/top-langs?username=anuraghazra

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)
Language stats algorithm
We use the following algorithm to calculate the languages percentages on the language card:

ranking_index = (byte_count ^ size_weight) * (repo_count ^ count_weight)
By default, only the byte count is used for determining the languages percentages shown on the language card (i.e. size_weight=1 and count_weight=0). You can, however, use the &size_weight= and &count_weight= options to weight the language usage calculation. The values must be positive real numbers. More details about the algorithm can be found here.

&size_weight=1&count_weight=0 - (default) Orders by byte count.
&size_weight=0.5&count_weight=0.5 - (recommended) Uses both byte and repo count for ranking
&size_weight=0&count_weight=1 - Orders by repo count
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&size_weight=0.5&count_weight=0.5)
Exclude individual repositories
You can use the &exclude_repo=repo1,repo2 parameter to exclude individual repositories.

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&exclude_repo=github-readme-stats,anuraghazra.github.io)
Hide individual languages
You can use &hide=language1,language2 parameter to hide individual languages.

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&hide=javascript,html)
Show more languages
You can use the &langs_count= option to increase or decrease the number of languages shown on the card. Valid values are integers between 1 and 20 (inclusive). By default it was set to 5 for normal & donut and 6 for other layouts.

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&langs_count=8)
Compact Language Card Layout
You can use the &layout=compact option to change the card design.

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=compact)
Donut Chart Language Card Layout
You can use the &layout=donut option to change the card design.

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=donut)](https://github.com/anuraghazra/github-readme-stats)
Donut Vertical Chart Language Card Layout
You can use the &layout=donut-vertical option to change the card design.

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=donut-vertical)](https://github.com/anuraghazra/github-readme-stats)
Pie Chart Language Card Layout
You can use the &layout=pie option to change the card design.

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=pie)](https://github.com/anuraghazra/github-readme-stats)
Hide Progress Bars
You can use the &hide_progress=true option to hide the percentages and the progress bars (layout will be automatically set to compact).

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&hide_progress=true)
Demo
Top Langs

Compact layout
Top Langs

Donut Chart layout
Top Langs

Donut Vertical Chart layout
Top Langs

Pie Chart layout
Top Langs

Hidden progress bars
Top Langs

WakaTime Stats Card
Warning

Please be aware that we currently only show data from WakaTime profiles that are public. You therefore have to make sure that BOTH Display code time publicly and Display languages, editors, os, categories publicly are enabled.

Change the ?username= value to your WakaTime username.

[![Harlok's WakaTime stats](https://github-readme-stats.vercel.app/api/wakatime?username=ffflabs)](https://github.com/anuraghazra/github-readme-stats)
Demo
Harlok's WakaTime stats

Harlok's WakaTime stats

Compact layout
Harlok's WakaTime stats

All Demos
Default
Anurag's GitHub stats

Hiding specific stats
Anurag's GitHub stats

Showing additional stats
Anurag's GitHub stats

Showing icons
Anurag's GitHub stats

Shows Github logo instead rank level
Anurag's GitHub stats

Shows user rank percentile instead of rank level
Anurag's GitHub stats

Customize Border Color
Anurag's GitHub stats

Include All Commits
Anurag's GitHub stats

Themes
Choose from any of the default themes

Anurag's GitHub stats

Gradient
Anurag's GitHub stats

Customizing stats card
Anurag's GitHub stats

Setting card locale
Anurag's GitHub stats

Customizing repo card
Customized Card

Gist card
Gist Card

Customizing gist card
Gist Card

Top languages
Top Langs

WakaTime card
Harlok's WakaTime stats

Quick Tip (Align The Cards)
By default, GitHub does not lay out the cards side by side. To do that, you can use this approach:

<a href="https://github.com/anuraghazra/github-readme-stats">
  <img height=200 align="center" src="https://github-readme-stats.vercel.app/api?username=anuraghazra" />
</a>
<a href="https://github.com/anuraghazra/convoychat">
  <img height=200 align="center" src="https://github-readme-stats.vercel.app/api/top-langs?username=anuraghazra&layout=compact&langs_count=8&card_width=320" />
</a>
<a href="https://github.com/anuraghazra/github-readme-stats">
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra&repo=github-readme-stats" />
</a>
<a href="https://github.com/anuraghazra/convoychat">
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra&repo=convoychat" />
</a>
👀 Show example
Deploy on your own
On Vercel
📽️ Check Out Step By Step Video Tutorial By @codeSTACKr
Since the GitHub API only allows 5k requests per hour, my https://github-readme-stats.vercel.app/api could possibly hit the rate limiter. If you host it on your own Vercel server, then you do not have to worry about anything. Click on the deploy button to get started!

Note

Since #58, we should be able to handle more than 5k requests and have fewer issues with downtime 😁.

Note

If you are on the Pro (i.e. paid) Vercel plan, the maxDuration value found in the vercel.json can be increased when your Vercel instance frequently times out during the card request. You are advised to keep this value lower than 30 seconds to prevent high memory usage.

Deploy to Vercel

🛠️ Step-by-step guide on setting up your own Vercel instance
On other platforms
Warning

This way of using GRS is not officially supported and was added to cater to some particular use cases where Vercel could not be used (e.g. #2341). The support for this method, therefore, is limited.

🛠️ Step-by-step guide for deploying on other platforms
Disable rate limit protections
Github Readme Stats contains several Vercel environment variables that can be used to remove the rate limit protections:

CACHE_SECONDS: This environment variable takes precedence over our cache minimum and maximum values and can circumvent these values for self-hosted Vercel instances.
See the Vercel documentation on adding these environment variables to your Vercel instance.

Keep your fork up to date
You can keep your fork, and thus your private Vercel instance up to date with the upstream using GitHub's Sync Fork button. You can also use the pull package created by @wei to automate this process.

💖 Support the project
I open-source almost everything I can and try to reply to everyone needing help using these projects. Obviously, this takes time. You can use this service for free.

However, if you are using this project and are happy with it or just want to encourage me to continue creating stuff, there are a few ways you can do it:

Giving proper credit when you use github-readme-stats on your readme, linking back to it. :D
Starring and sharing the project. 🚀
paypal.me/anuraghazra - You can make a one-time donations via PayPal. I'll probably buy a coffee tea. 🍵
Thanks! ❤️

https://vercel.com?utm_source=github_readme_stats_team&utm_campaign=oss

Contributions are welcome! <3

Made with ❤️ and JavaScript.

About
⚡ Dynamically generated stats for your github readmes

github-readme-stats.vercel.app
Topics
serverless dynamic hacktoberfest readme-generator profile-readme readme-stats
Resources
 Readme
License
 MIT license
Code of conduct
 Code of conduct
Security policy
 Security policy
 Activity
Stars
 72.2k stars
Watchers
 283 watching
Forks
 24.2k forks
Report repository
Sponsor this project
@anuraghazra
anuraghazra Anurag Hazra
https://www.paypal.me/anuraghazra
https://www.buymeacoffee.com/anuraghazra
Learn more about GitHub Sponsors
Used by 100
@mahshid1378
@ahmed-on391
@aestdile
@rcptok25
@briankaboyi
@JoseAn2004
@erasernoob
@AbnerDiniz90
+ 92
Contributors
278
@qwerty541
@dependabot[bot]
@anuraghazra
@rickstaa
@nathanchu
@github-actions[bot]
@Zo-Bro-23
@omidnikrah
@nombrekeff
@florianbussmann
@JounQin
@lrusso96
@oscard0m
@fabianocouto
+ 264 contributors
Languages
JavaScript
99.8%
 
Shell
0.2%
Footer
© 2025 GitHub, Inc.
<!--
**Gouravsharma20/Gouravsharma20** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
