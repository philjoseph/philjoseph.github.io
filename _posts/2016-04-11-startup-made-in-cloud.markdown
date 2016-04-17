---
layout: post
title:  "Startup made in cloud"
date:   2016-04-10 18:21:31
categories: business, cloud
author: "Philippe Cohen"
---
The first lesson I am taking from my recent startup experiences is that the Cloud and all the services it offers makes the launch a new startup from scratch a trivial and unexpensive exercise. Basically all you need today to launch a new development operation is simply a couple of great developers (I am still not hiring much over the cloud, but this worth another post), good laptops and fast internet connections. No need for servers, no server room, no RAID disks, no backup devices, no switches, no hubs, no sysadmin, no firewall, no [DevOps](https://en.wikipedia.org/wiki/DevOps){:target="_blank"} engineers, no production manager, no [clearcase VOBs](https://en.wikipedia.org/wiki/Rational_ClearCase){:target="_blank"}, no source control administrators...

So let’s detail all what it takes to start a new startup operation.

<div style="text-align:center" markdown="1">
![](/assets/startup.png)
<br>
</div>

## Internet presence
First thing you need a domain name. You can buy one from any domain registrars. This can cost you a simple 10 dollars if you are creative enough to come with a new name. You can even buy your domain directly via Google apps. I’ve gone via [Godaddy](https://www.godaddy.com/){:target="_blank"} (note that I am not convinced this is the best one). You will also need to decide where to manage your DNS, I’ve finally opted for [AWS R53](https://aws.amazon.com/route53/){:target="_blank"} that is great even not easy to use, you will likely need to issue SSL (and maybe code signing) certificate, and I’ve used GoDaddy and setup a [Deluxe wildcard certificate](https://www.godaddy.com/help/which-ssl-do-i-need-5342){:target="_blank"}. All this can be done in a couple of days, except the SSL certificate that will likely take some back and forth for the authentication process.

<div style="text-align:center" markdown="1">
![](/assets/ChooseDomainName.jpg)
<br>
</div>

## Email and more...
Once you have a domain, you need set up emails, calendar, contacts and document collaboration for your team. I had no much hesitations and used [Google app](https://apps.google.com/){:target="_blank"}. For a $4 per user and per month, and with a minimal admin effort (still their admin console could be improved), you have email, calendar, and documents collaboration. I am myself not a fan of Google UX style so I am using the Apple apps on my macbook connected to Google mail, calendar and contacts. Some will prefer Office 365 but I have to say that I just glad to not use back Outlook again! Also Google docs are really just great in term of collaboration much better than all of what Microsoft offers so far.Most of the dev team was on Linux and some on Windows, everyone picked up the right email and calendar clients for environment. No need to mention that Android and iPhone were seamlessly accessing the apps with no special setups.
<div style="text-align:center" markdown="1">
![](/assets/googleapps.png)
<br>
</div>


## Blog and static sites made trivial
When I decided to launch the corporate web site and a blog, I was first sure to go with Wordpress and e of the hosting offers, selecting a template among the hundreds out there, and setting up my WordPress environement with the help of a consultant and also
paied some $50 yearly for hosting. [Raphaël](https://il.linkedin.com/in/raphael-boukara-b3433a18){:target="_blank"} suggested me to use [jekyll](https://jekyllrb.com/){:target="_blank"} that together with the free [Github](https://github.com/){:target="_blank"} hosting make it very convenient, completely autonomeaous and free solution. I fall in love with Jekyll and never met his Mr Hyde counter part.
<div style="text-align:center" markdown="1">
![](/assets/blog.jpg)
<br>
</div>

## Agile project management 
Now we are all set, it was time to start working on some real development tasks. We selected [Trello](https://trello.com/){:target="_blank"} for our project management. Trello is basically a [Kanban board](http://leankit.com/learn/kanban/kanban-board/){:target="_blank"}, so simple that you would think it’s almost stupid. No mistake - Trello is a very powerful tool. Simplicity is indeed its first strength but, the built-in collaboration capacity, the power of each ticket with the attachments, the checklists, the labels, give you a great way to run your projects. 

> As a side remark for UX folks: I see the simplicity of Trello as inspiring. Users discover the power as they use the product more and search for more features. They are not overwhelmed with a bunch of features they are not yet ready to discover.

We ran on the free version for more than one year, and then discovering the various [power ups](https://trello.com/power-ups){:target="_blank"} Trello is offering, I’ve switched our team to their [business class](https://en.wikipedia.org/wiki/Business_class){:target="_blank"}. This way we had each development ticket connected to the [github pull requests](https://help.github.com/articles/using-pull-requests/){:target="_blank"}, our documentation board well integrated with Google docs, our Support tickets linked to the Salesforce case and there are many more... 

Trello is a masterpiece in our agile operation because of its simplicity. Thanks to its collaboration features, it makes it very easy to share project dynamics with different stake holders and to collaborate with external people. We succeed to work with teammates on 3 different continents and with up to 11 hours difference, in a very cohesive way.

Did I mention that their mobile app is just great and found myself answering questions from developers while walking to customer meetings.
<div style="text-align:center" markdown="1">
![](/assets/DilbertAgileProgramming.jpg)
<br>
</div>

## Instant messaging and much more
I was using Skype for a while and used a bit Google hangouts. [Slack](https://slack.com/is){:target="_blank"} is going much beyond those tools. 

* Like Skype and Hangouts, Slack enables you to instant message (direct message - DM) with your teammates and make it convenient to have organize your contact  per organisation and teams. The facility to drag and drop media contents and have link preview make it a first class instant messaging. The recent beta of the voice and video communication makes it a leading communication tool.  

* Open channels is a nice concept, everyone can decide if to subscribe or not to an open channel. That is a significant change in the communication culture, where the sender do not have to decide who to include in his/her post but rather each one decide if the topic is of interest. It’s a [publisher-subscriber pattern](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern){:target="_blank"} versus point to point communication tools like emails and phone. So using slack reating channels, that are topics such as design, back-end, team events, … where each one can subscribe or unsubscribe (more open than a whatsapp group) you start realizing the power of the tool. Basically you do not have to decide to who you send a message, people interested in receiving it will just got it. Note you can also have private channels that are reserved to invited people.

* This is not all. We integrated Trello alerts, and all systems sending alerts and notifications, such as our DevOp monitors, Logentries, NewRelic, Honeybadger... (more about DevOp in another post). Then within one tool, we had all our communications regrouped and it makes ourselves much more efficient than reading emails. Also the powerful search enabled us to find and share all contents so quickly. I see more and more people managing their meetings and communication around Slack and believe it is one of the most interesting change in communications since the failing attempt of Google with Threads. 

<div style="text-align:center" markdown="1">
![](/assets/slack.png)
<br>
</div>

Bottom line, the cloud is changing the way we start a new operation, the way we run projects and communicate, the money we spent on infrastructures and most important its change our user experience. 

> Note: I did not write about the sales operation, since we used Salesforce.com that is expensive and not offering a great user experience. I've looked for a good, nice, simple and cheap CRM over the cloud with no clear findings. If you have a recommendation, please post it here.

In the next post, I will talk about the impact of the cloud on the development and the DevOp perspective. 
