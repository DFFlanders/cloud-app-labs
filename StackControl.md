# StackControl Application Laboratory

Welcome to the OpenStack Cloud App Lounge!  Below you will find the third (3of6) app lab challenges.  Each lab is a playful way to see if you have what it takes to be a ['Cloud Application Engineer'](/cloud-application-engineer.md) - the future of apps. 

Don't forget to [setup your laptop with the OpenStack powered cloud of your choice](/prereq)

![Cloud apps are the future...](https://pbs.twimg.com/media/CuJSGSrUEAAXoeK.jpg)

## Learning context for completing the lab
 - A international consortium of University professors are releasing a series of scientific discoveries which are highly sensitive and likley to be contested (akin to WikiLeaks data but for the Scientific sector).  You can either use [the app which the professors have created](http://developer.openstack.org/firstapp-shade/introduction.html) or select another app which can host static HTML Web pages (e.g. wordpress, plone, etc).
 - You need to upload an application to the cloud (via shade) which can host mirrors of the content in multiple locations.  NB for this excercise your applications do not need to be sync'd between different datacenters (aka state/less), as we'll cover app state in a future lab.  The professors just want to make sure the content is online and easy to access/read/copy.
 - Get additional points for each datacentre around the world which hosts an applicaiton serving the professors Web pages.

# Lab learning objectives _(by completing this lab you will know how to...)_
 - [x] ...controle the hardware resources within a datacenter's (cloud) via ReSTful resources requests (CRUD).
 - [x] ...initialise an instance (virtual machine) atop the datacenter's infrastructure.
 - [x] ...upload an application to VM and place it on a public network for access via a Web URL.

## Win StackerPoints for completing this lab:
  - Win StackerPoints by tweeting a public URL(IP) showing an application running on the cloud which is able to display webpages. Hint: python SimpleHTTPServer --> index.html
  - Get one of the [Cloud App Pros](https://docs.google.com/presentation/d/1RBtAOjxmUh97fXrJlowvqVNmq2-8FxvBIHx2Dts1Jh8/pub?start=true&loop=true&delayms=1000) to "❤" your tweet.
  - Once an App Pro has +1'd your tweet, come and show your ❤'d tweet to the helpdesk in the Cloud App Lab Lounge in the Marketplace (Expo Hall) to claim your [StackerPoints](/StackerPoints).

## Ingredients you'll need for completing this lab:
  - [Building on the previous lab's library (os-cloud-config.py), you'll install and use the shade library to access and control two or more of the OpenStack powered dataceters of your choice](https://github.com/openstack-infra/shade)
  - [To upload an application to the cloud you'll neeed to learn some shade usage commands](http://docs.openstack.org/infra/shade/usage.html).  Hint `image = cloud.create_image()`
  - Once you have your virtual machine, container and/or baremetal instance substantiated you'll need to upload an application to it.
  - If you'd like an application to work with which we'll be using in future labs, feel free to use this [application which serves scientific fractals](http://developer.openstack.org/firstapp-shade/introduction.html#complete-code-sample).

## Lab pros who can help you complete this lab:
Stuck on this lab, need some help to solve?  [Ping one of our Cloud App Lab Pros on Twitter/IRC](https://docs.google.com/presentation/d/1RBtAOjxmUh97fXrJlowvqVNmq2-8FxvBIHx2Dts1Jh8/pub?start=true&loop=false&delayms=2000). Hint: Community driven Open Source is about knowing *who* as much as it is about knowing *what*.

Recommended _cloud app pros_ who can help (via Twitter/IRC):
 - @BrunouyVanMorel
 - @SquidBoylan
 - @JoannahHuang
 
# Solving the lab
Having trouble?  Sit back and watch someone else solve this lab learning challenge ;-)

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/JyQHoDoypGM/0.jpg)](http://www.youtube.com/watch?v=YOUTUBE_JyQHoDoypGM)

