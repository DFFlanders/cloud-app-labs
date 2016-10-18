# StackScale Application Laboratory

Welcome to the OpenStack Cloud App Lounge!  Below you will find the fourth 'cloud app lab' challenge.  Each lab is a playful way to see if you have what it takes to be a ['Cloud Application Engineer'](/cloud-application-engineer.md) - the future of apps.

Don't forget to [setup your laptop with the OpenStack powered cloud of your choice](/prereq).

![State or stateless? The key question for every cloud applicaiton engineer to understand.](https://pbs.twimg.com/media/Cudphb2VMAMjaO3.jpg:large)

## Learning context for completing the lab
 1. Imagine (fictionally): a recent scientific dsicovery from the CERN laboratories in Switzerland have revealed that fractals generated from prime numbers can predict the origins of the universe! 
 2. A group of proffessors have written an applicaiton which generates fractals, however their cloud application is being inundated with requests from researchers worldwide who want to generate fracts.
 3. The professors have hired your team to help scale their fractal applicaiton so that it can dynamically scale and generate as many fractals as are being requsted by Physics and Mathematics departments worldwide!
 4. Perhaps most importantly, the professors (being poor researchers) need you to demonstrate you are using datacenters which are cost effective and competitive with one another to help keep costs down (and to assure government research funding is being distributed to multiple infrastructure providers).
 5. Can your team enable this simple cloud application to scale globally while still keeping the data locally?!

# Lab learning objectives _(by completing this lab you will know how to...)_
 - [x] ...re-factor your cloud application architecture to have multiple 'app workers' which can be dynamically scaled and placed at any OpenStack-powered-datacentre worldwide.
 - [x] ...meet community members who have built and maintained various stateless enterprise applications in production.
 - [x] ...understand the concept of 'state' (stateless/statefull) applications and the implications for different design patterns for managing various _cloud app statless-ness_.

## Win StackerPoints for completing this lab:
  - Tweet a picture showing that your application is working in multiple datacenters, i.e this could be a picture of your network topology, it could be a video of your IDE stopping/starting workers, etc. 
  - Get one of the [Cloud App Pros](https://docs.google.com/presentation/d/1RBtAOjxmUh97fXrJlowvqVNmq2-8FxvBIHx2Dts1Jh8/pub?start=true&loop=true&delayms=1000) to "❤" your tweet showing your app working as statelessly!
  - Once an App Pro has +1'd your tweet, come and show your ❤'d tweet to the helpdesk in the Cloud App Lab Lounge in the Marketplace (Expo Hall) to claim your [StackerPoints](/StackerPoints).

## Ingredients you'll need for completing this lab:
  - [ ] The [Fractals Application is avaialble here](http://developer.openstack.org/firstapp-shade/introduction.html), including instructions for a possible statelss architecture.
  - [ ] You'll need to utilise the Shade SDK/API calls to manage your application accross different OpenStack-powered-datacenters.
  - [ ] Make sure you are managing your account details for each cloud via our clouds.yaml file and os-cloud-config.py library.
  - [ ] Bonus points: pay attention to where your fractal workers are putting the fractals once they are generated.

## App pros who can help you complete this lab:
Stuck on this lab, need some help to solve?  [Ping one of our Cloud App Lab Pros on Twitter/IRC](https://docs.google.com/presentation/d/1RBtAOjxmUh97fXrJlowvqVNmq2-8FxvBIHx2Dts1Jh8/pub?start=true&loop=false&delayms=2000). NB Open Source is about knowing *who* as much as it is about knowing *what*.

Recommended _cloud app pros_ who can help (via Twitter/IRC):
 - @BrunoMorel
 - @VKMC
 - @SquidBoylan
 - @Serg
 - @Chris Aedo...
 - @Marcella...
 
# Solving the lab
Having trouble?  Sit back and watch someone else solve this lab learning challenge ;-)

[![Screencast showing how to divide out the state of your app workers so you can scale based on demand or location of your app being used.](http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](http://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)
