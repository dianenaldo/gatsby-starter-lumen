---
template: post
title: Fix Bug "Unknown field socialImage" on Gastby Templates
slug: /post/bug-unknown-field-social-image
draft: false
date: 2019-09-21T18:55:17.304Z
description: >-
  May Bug sa Gatsby post-template.js at page-template.js graphql queries, papanu
  ba to ayusin?
category: Bug Fixes
tags:
  - Gatsby
---
Habang nagde-deploy ako ng aking updates sa gatsby blog site ko napansin ko na biglang nakaka-error sa page-template.js na file. At ang sabi sa error ay ganito **Unknown field 'socialImage'** blah blah blah, nung una ang akala ko ay nabura ko lang lahat ng pages kaya nagre-reklamo si Graphql na wala na syang mahanap na socialImage field. pero nung sinubukan ko ng ibalik ang isa sa mga page na na-delete ko eh hindi parin gumagana! anyare?? 



I being frustrated kasi wala akong mahanap na documentation or forums na pwdeng makatulong sa problema ko. napapanung tuloy ako bakit ako lang ang nagkaka-error ng ganito?? bakit ako lang!



So....

Ginawa ko kung anu man ang ginagawa ng isang matinong developer, manghula at mag-delete ng bug sa code. madali lang naman hanapin yung socialImage field na yan sa codes, ang tanung lang is tama ba e-comment out o e-delete yung line of code na yun.

Eto piece of advice, sa pagde-debug ng code eh maganda magsimula basahin muna ang lahat ng dependency ng code na balak mong burahin, check first kung saan saan sya ginamit. then after if make sense at sa tingin mo na dapat malawa na sya sa dun then go with the deletion.  

What make my decision final is that I don't use this field anywhere on my blog site and I'm not planning to use it anytime soon.

here the graphql query looks like with the socialImage field in it:

> src/templates/page-template.js

```
export const query = graphql`   query PageBySlug($slug: String!) {     markdownRemark(fields: { slug: { eq: $slug } }) {        id         html         frontmatter {           title           date           description           socialImage       }   }}`;
```

I deleted the **socialImage** field from this query and it fix the bug.



Anyway that's it, I hope you learn something from this post and hopefully this code will not haunt me in my sleep.
