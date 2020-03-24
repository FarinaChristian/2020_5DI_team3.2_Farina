# System Documentation

# Team 4

# 1 Introduction

The SF-Agriculture application allows users a simple way to manage their field and their agricultural yield. This document will provide instructions for accessing the application code and installing it into a simulator or compatible device.

# 2 Setup Proxy Server

A Unix/Linux based server with Internet connectivity is required for the web proxy. 

1. 1 Obtain the current Perl distrubution
  2. 1.1 Install perl modules from CPAN
2. 2 Install IIS.
  1. 2.1 Configure apache with https support
        1. 2.1.1 Configure IIS with cgi support
      1. 2.1.1.1 Place perl proxy software in the designated cgi-bin directory

# 3 Access To Your Profile

Internet access is required, to enter your personal profile you must first register. Once the user has created his account he will have access to additional features for the calculation of his agricultural yield.

# 4 Install on Simulator or Device

## 4.1 Required Components

Our application can be used on any device with any operating system. We suggest using fairly performing devices as the site may be slow to load because it contains many high definition images.

# 5 System Maintenance

## 5.1 Objective-C Code

The user interface consists of four tabs for viewing information, in addition to the login screen. There are two main web pages visible to all users, and another two pages visible only to users registered with our service. There are two additional XML files: the root view of the application and the navigation view of the tab bar. All information regarding users and their fields are saved in our databases.

On first launch, the application displays the login screen. Once the user has logged in, the view switches to the tab bar, which is displayed at the bottom of the screen. The view of the tab bar allows the user to move between the tabs mentioned above and houses the four secondary views for each type of information.

The logic in each class of view controllers mainly performs the task of extracting the appropriate data from XMLParser, formatting it and displaying it in the correct fields. The access controller class also contains logic for storing user credentials on the site registration page (personal area).

## 5.2 Perl Proxy Code

Our proxy server consists of a perl cgi, executed by apache when a specific POST is received via https. The perl code accesses managemyid using the users' credentials (provided in POST). From there, the code acquires an https redirect and uses the unique URL in the redirect to request the account balance and history. This is accomplished in three separate https transactions with managemyid.

As information is collected from the second two transactions with managemyid, the perl script generates XML and sends it to the C-target parser on the iOS device through the tcp stream (still open).