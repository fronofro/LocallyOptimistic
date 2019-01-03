---
author: Michael Kaminsky
title: "The Analytics Engineer"
publishDate: "2019-01-31"
draft: True
tags: 
 - analytics
 - software
 - data
 - engineering
---

The landscape of the data and analytics world is shifting rapidly. In many companies, the roles and responsibilities  of data engineers, analysts, and data scientists are changing. This change has created the need for a new role on the data team which some of have taken to calling the "analytics engineer". 

<!--more-->

The analytics engineer sits at the intersection of the skill sets of data scientists, analysts, and data engineers. They bring a formal and rigorous software engineering practice to the efforts of analysts and data scientists, and they bring an analytical and business-outcomes mindset to the efforts of data engineering. It's their job to build tools and infrastructure to support the efforts of the analytics and data team as a whole.

Before we dive further into the role, we should cover some background on the "traditional" roles on the data team[^1]. 

* Data engineers: traditionally, this has been a "plumbing" job of moving bytes from point A to point B. They were concerned with building robust and scalable infrastructure for ingesting and storing data, but generally did not concern themselves with "business logic" -- once the data were in the warehouse, it wasn't there problem any more.
* Analysts: traditionally, this has been a reporting and pure analysis job. Using a little SQL and a lot of excel, analysts would maintain dashboards and perform one-off strategic analyses to support key business initiatives
* Data scientists: somewhat of a mixed bag, however data scientists traditionally spent their time using statistical programming languages (like R or SAS) to perform more complicated or sophisticated analyses. They would perhaps "prototype" machine learning models that get handed off to the "real engineers" for implementation in production.

In the last few years, we've seen a lot of exciting developments in the analytics domain that have caused a shift in these traditional responsibilities. They are:

* The rise of MPP SQL data-warehousing technologies like Redshift, BigQuery, and Snowflake
* The birth of data-pipelines-as-a-service companies like Stitch and Fivetran
* The advent of SQL-first BI tools like Looker, Mode, and Periscope
* The emphasis companies are putting on building data-driven products that rely on micro-targeting and machine learning algorithms for prediction and personalization.

The first two, taken together, have shifted the role of analysts dramatically. Nowadays analysts _must_ know how to write SQL, use git/github, and generally spend a majority of their time _writing code_. While they aren't necessarily trained as software engineers, they are now responsible for managing substantial codebases. Similarly, while data engineers used to spend a lot of time split between building new data integrations between systems or working on platforms for scalable computation, most of that work can now be offloaded to Stitch/Fivetran (integrations) or to the warehouse itself (just let BigQuery figure out the optimal query plan). Finally, data scientists have suddenly become responsible for managing sophisticated production systems that are making real-time productions with significant business impact.

So what are the new roles and responsibilities?

* Data engineers: still responsible for data infrastructure and plumming code, but the team is now generally much smaller than it was in the past. Many companies can get by just using contractors and consultants in the beginning, and they may only need one or two data engineers to "fill in the gaps" of what they can't purchase from off-the-shelf solutions
* Analysts: In addition to performing ad-hoc analyses, analysts are responsible for programming and managing BI tools and writing some ELT jobs (in Looker PDTs or via a tool like DBT)
* Data scientists: In addition to doing one-off research tasks, data scientists are managing complex pipelines of data cleaning and orchestration feeding into machine learning models and sophisticated testing platforms.

Those who have worked in an organization like this before have likely felt the pinch of a missing role. While data scientists and analysts are writing a lot of code, being great software engineers isn't what they've been trained for and it often isn't their first priority. Similarly, while data engineers are great software engineers, they don't have training in how they data _are actually used_ and so can't always partner effectively with analysts and data scientists. 

--------------------

The new jobs:

* data engineer
* analysts
* data scientists

With all of these roles more frequently touching production code, there's a need for a role that can sit in between these functions and ...

[^1]: I realize I'm painting with a pretty broad brush here and these descriptions will not capture everyone's experience at every different company. This does however reflect a lot of what I've experienced and discussed with people across a wide range of companies and disciplines.