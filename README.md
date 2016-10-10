# Cloud App Labs at OpenStack Summit Barcelona 2016

![Cloud App Labs at the OpenStack Summit in Barcelona Spain](https://pbs.twimg.com/media/CuN700EWEAAo4xK.jpg:large)

Welcome to the OpenStack Summit.  The following 'Cloud App Labs' are part of the growing 'OpenStack Application Academy' and will be located in the Summit Marketplace (aka Expo Hall). This repository contains a series of 'Cloud App Labs' to help you get self-started with becoming a _cloud application engineer_ - the future of apps development.

TL;DR = Learn the skills to become a 'Cloud Application Engineer' - ask Q's anytime by sending a tweet which includes [#CloudApp](https://twitter.com/hashtag/cloudapp) + your question which one of our [Cloud App Pros](https://docs.google.com/presentation/d/1RBtAOjxmUh97fXrJlowvqVNmq2-8FxvBIHx2Dts1Jh8/pub?start=true&loop=true&delayms=1000) will answer.

Overall Learning Objectives (_by completing these labs you will know how to..._)
 - [x] ...work as part of the growing cloud app community, to understand the significance of working as part of a multi-factor cloud application team.(NetEng, SysAdmin, DevOpps, AppDev, UX, etc).
 - [x] ...be inspired to build cloud apps which are cross-cloud (not locked into single cloud operating infrastructure systems).
 - [x] ...make cloud apps which are simple at the start: constrain their state so they can be further configured as they evolve (to become stateless aka cloud native).
 - [x] ...know where to go to for further learning resources and community ideas for building the cloud apps of the future.

The overall aim of the cloud apps lab lounge is to connect you with likeminded cloud application community members who are evolving the thinking on how to engineer cloud apps which will work interoperably accross various open cloud infrastructures. AKA say "'no' to cloud app lock-in".

Depending on your skill level, each lab will take anywhere from five to forty-five minutes (faster for those who know how to _ask for help_).
Labs are designed to start easy and get more difficult, so as to keep you _playfully challenged_.

You can get help on each lab by simply hanging out in the "Lab Lounge" and asking for help at the info-desk; or you can ask one of our [app pros](https://docs.google.com/presentation/d/1RBtAOjxmUh97fXrJlowvqVNmq2-8FxvBIHx2Dts1Jh8/pub?start=true&loop=true&delayms=1000) who will be on-hand to help.  Also, get help by tweeting your question by using the [#cloudapps](https://twitter.com/hashtag/cloudapps) hashtag via twitter/irc (we'll continually monitor #OpenStack channels).

**Best of all, win points by completing labs which will earn you Stacker swag!**
![Win Stacker Swag by completing these Cloud App Labs](https://pbs.twimg.com/media/CuNYDXsWIAARjHb.jpg:large)

The process for completing labs and earining Stacker points is simple:
 1. select a lab (below) to complete;
 2. get help to complete the lab;
 3. show your lab result to the community to get points;
 4. use your points to claim Stacker swag at the 'App Labs' lounge.
 5. Repeat by completing more labs (see step 1)

To get you started you'll need to have the following pre-requisites:
 * a laptop with wifi access whose SSH ports are open.
 * very basic Python scripting skills
 * an account on one of the many OpenStack public clouds: if you don't have one, we have one for you.
 * an SSH key and basic understanding for how to apt-get install applications on the cloud (only very basic).
 * an understanding for the basics for making URL based (ReSTful) code calls to a datacenter's API endpoints.
 * #!--> [Setup your laptop to work with an OpenStack powered datacenter](/prereq.md)

# List of Cloud Application Laboratories
Let's get started, pick a lab:

## Cloud App Lab no.1 - [StackTour: an overview of OpenStack projects as per the buttons they relate to on the Web dashboard.](/StackTour.md)

About this lab:
 - [x] _Skills you'll learn_ = which buttons on the OpenStack dashboard (Horizon) connect with the other core OpenStack projects (Nova, Neutron, Cinder, Swift, Glance, etc).
 - [x] _Copmmunity you'll meet_ = people who are actively getting their users to launch their own applications using the dashboard and basic scripting skills.
 - [x] _Point's you'll score_ = up to +10 points for completing this lab. [What can I win with 10 StackerPoints?!](/StackerPoints.md)

## Cloud App Lab no.2 - [StackEntrance: having your own personal entrace to all OpenStack public clouds worldwide](/StackEntrance.md)

About this lab:
 - [x] _What you'll learn_ = how to configure your laptop to control a datacenter, so that you don't have to use a Web based dashboard; instead, use simple python scripts to get access to datacenters (powered by OpenStack worldwide). Yes that's right, one simple file is all you need to access hundreds of clouds (i.e. clouds.yaml via os-cloud-config.py)
 - [x] _Community you'll meet_ = people who are helping engineers shift their skills to be able to: a.) authenticate via command line, b.) use of YAML as a simple structured document for storring login details, and c.) basic (beginner) control of a datacentre via command line API calls.
 - [x] _Points you'll score_ = +10 points for completing this lab. [What can I win with my StackerPoints?!](/StackerPoints.md)

## Cloud App Lab no.3 - [StackControl: how to upload and control a muti-factor application to OpenStack-powered datacenters arounds the planet](/StackControl.md)

About this lab:
 - [x] _What you'll learn_ = how to upload an application to a datacentre cloud using basic command line python code.
 - [x] _Community you'll meet_ = people who understand how to enable application developers to use basic cloud skills for: a.) controlling a datacentre via command line API calls, and b.) using a simple python library (shade).
 - [x] _Points you'll score_ = +10 points for completing this lab. [What can I win with my StackerPoints?!](/StackerPoints.md)

## Cloud App Lab no.4 - [StackCentres: installing an application with multiple workers at different datacenter locations around the world.](/StackCentres.md)

Aboout this lab:
 - [x] _What you'll learn_ = install an application whose data (state) needs to be maintained seperate from the stateless jobs of the application workers. 
 - [x] _Community you'll meet_ = advanced applicaiton engineers who are experimenting with how to best build applications which are stateless in their design, but stateful in their storage of data long term and for use by other applications.
 - [x] _Points you'll score_ = +25 points for completing this lab. [What can I win with my StackerPoints?!](/StackerPoints.md)

## Cloud App Lab no.5 - [StackData: attaching storage to your multi-factor app, undertanding state/less app architectures.](/StackData.md)

About this lab:
 - [x] _What you'll learn_ = Building on Lab no.4 you'll start to utilise the block (volume) storage of OpenStack so your application can share it's data with other application in your enterprise.  
 - [x] _Community you'll meet_ = engineers who manage application and operational systems whose data is required to be available for the long term business of the enterprise.
 - [x] _Points you'll score_ = NN points [What can I win with my StackerPoints?!](/StackerPoints.md)
 
## Cloud App Lab no.6 - [StackHeal: start to create self-healing workers to monitor and rebuild different parts of your cloud applicaiton in situ.](/StackHeal.md)

About this lab:
 - [x] _What you'll learn_ =
 - [x] _Community you'll meet_ = advanced, understanding of application architectures and orchstration frameworks...
 - [x] _Points you'll score_ = +15 points for completing this lab. [What can I win with my StackerPoints?!](/StackerPoints.md)

# Future Cloud App Labs coming soon!
Stay tuned for these future cloud app labs...

## Cloud App Lab no.7 - StackContainers: start splitting out the state of your app workers to be more agile (self healing) as containers which can dynamically shift accross datacentres worldwide.
About this lab:
 - [x] _What you'll learn_ =
 - [x] _Community you'll meet_ =
 - [x] _Points you'll score_ = 

## Cloud App Lab no.8 - [StackDock: launch Docker on OpenStack then launch an a cloud app within Docker](/StackDock.md)
About this lab:
 - [x] _What you'll learn_ =
 - [x] _Community you'll meet_ =
 - [x] _Points you'll score_ = 
 
## Cloud App Lab no.9 - [StackPod: launch Kubernetes on OpenStack and get a cloud app working within K8S](/StackPod.md)

About this lab:
 - [x] _What you'll learn_ =
 - [x] _Community you'll meet_ =
 - [x] _Points you'll score_ = 
 
# Cloud App Lab no.Z - StackFoo: do you have an idea for a self-paced cloud app lab, click the branch button now ;0)
Go on, just 'fork/pull' now :)


