---
template: post
title: Create a Gatsby Blog Site
slug: gatsby-blog-site
draft: false
date: 2019-09-21T15:06:58.383Z
description: >-
  Anu nga ba ang Gatsby? at papanu gumawa ng blog site gamit eto? bibigyan natin
  ng simpleng explanation gamit ang salitang taglish o tagalog at english.
category: Progressive Web Application
tags:
  - Gatsby
---
Okay ang **Gatsby** o **GatsbyJS** sa simpleng salita ay isang tools na pangawa ng blog site, website, eCommerce site, web application etc. karamihan ngaun ng mga web developer ay nag-transition na sa paggamit ng gatsby sa kani kanilang project, kasi nga naman mas mabilis at mas akma sa pangangailangan ng mga progresibong web application ngaun.

Mejo magiging technical tayo ngaun ng konti, subukan kung pahapyawan at ipaliwanag kung papanu ba gumagana etong Gatsby. Isang rason kung bakit ginawa ang Gatsby ay para merong mag translate ng mga data galing **GraphQL**. ang GraphQL ay uri ng query language na mga alien lamang ang nakakaintidi, wag kang magalala hindi naman natin kelangan maintindihan ngaun yang graphql graphql na yan, basta ang alam natin si Gatsby ay marunong mag-translate ng salita ng mga alien. ang data ay posibleng manggaling sa iba't ibang source o database, at eto ay nagpo-produce ng iba ibang format, salita ng mga alien. at dito na nga pumapasok si gatsby para mag-translate.

Tama na ang sasat simulan na natin gumawa ng blog site! una kailangan nating mag-install ng **Node.js**, **Git** at **Gatsby CLI**. 

Buksan ang iyong **Terminal** sa Linux o **Command Prompt** sa Windows

Install Node.js on Linux

```
sudo apt-get install nodejs
```

for Windows:  <https://treehouse.github.io/installation-guides/windows/node-windows.html>

Install GIT on Linux 

```
sudo apt-get install git
```

for Windows:  <https://www.atlassian.com/git/tutorials/install-git#windows>

Install Gatsby CLI on Linux/Windows

```
npm install -g gatsby-cli
```

tapos na tayo mag-install lahat ng prerequisites, mag-create na tayo ng Gatsby blog site!

```
gatsby new sampol-blog-site https://github.com/alxshelepenok/gatsby-starter-lumen 
```

pagkatapos pumasok sa loob **sampol-blog-site** directory

```
cd sampol-blog-site
```

patakbuhin ang blog site locally o sa iyong computer

```
gatsby develop
```

pwde mo na ngaun mabisita ang iyong blog site sa: [http://localhost:8000](http://localhost:8000/)

Enjoy!



Okay meron na tayong simpleng blog site, anu na ang susunod? syempre kailangan natin lagyan ng content at baguhin ang ibang detalye tulad ng blog owner name, profile picture, social media links etc. at papanu ba eto magkakaroon ng sarili nyang domain? Abangan sa susunod at tatalakayin natin ang patungkol sa Headless CMS, Blog Configuration, Deployment to Netlify at Setting up your custom domain from Namecheap.



Para sa karagdagang kaalaman bisitahin ang mga references: 

<https://www.gatsbyjs.org/tutorial/part-zero/#using-the-gatsby-cli>

<https://github.com/dianenaldo/gatsby-starter-lumen>
