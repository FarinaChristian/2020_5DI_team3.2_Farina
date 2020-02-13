# Software Requirements Specification

December 4, 2019

Version 1



Prepared by:

SF-Agriculture



Revision History

| Version | Date | Name | Description |
| --- | --- | --- | --- |
| 1 | 09/23/10 | Pertile Gian Marco | Initial Document |
|   |   |   |   |



# 1 Introduction

## 1.1 Overview

The SF Agricolture web application will be an online service available on every platform. This web application will provide the customer with a detailed description of the agricultural yield of their land using the data provided by the user concerning the type of land, its geographical location, type of seed used and average seed cost.

This document provides information on the requirements for the SF Agricolture web application. The objectives, scope and definitions of the project are reported in the introduction. Design constraints and environmental applications are described in the following section. Non-functional requirements are indicated for later verification. Functional requirements are provided to show the features of the system and the expected user interaction.

## 1.2 Goals and Objectives

1. The overall goal is to provide an efficient way to keep track of the performance of your agricultural business

   · Provide a mobile interface to control and manage your farm

   · It works in a simple and intuitive way.

   Provide entrepreneurs with a real-time description of the progress of their agricultural enterprise

## 1.3 Scope

The SF Agricolture application will provide users with the possibility to verify the agricultural yield of their land from any computer connected to an internet network or from a mobile device. Users will be able to verify the profit of their own farm by accessing the
our SFAgricolture.com site via any search engine.

## 1.4 Definitions

**SF Application** – the product that is being described here; the software system specified in this document.

**Project** – activities that will lead to the production of the SF Agricolture web application.

**Client** – the person or organization for which this SF Agricolture application is being built.

**User** – the person or persons who will actually interact with the SF Agrcolture web application.

**Use Case **: describes a goal-oriented interaction between the system and a customer. A use case can define different variants called scenarios that determine different paths through the use case and generally different results.

**Developer** – the person or organization developing the system, also sometimes called the supplier.

# 2 General Design Constraints

## 2.1 SF-Agriculture Web Application Environment

The SF-Agriculture product will include access to a web page designed to work for any device connected to the internet. This application interfaces with a proxy server designed by us. This proxy server interfaces with the SFAgricolture.com website. The proxy server will allow more efficient maintenance of the software system.

## 2.3 User Characteristics

**Roo Bucks Users** : Farmers and entrepreneurs can use the product using a smartphone, tablet or personal computer. Users interact with the web platform to use the service effectively.

## 2.4 Mandated Constraints

The application requires an initial registration for every user who wants to use the web application. At each access to the page the user must log in before being able to use the service.

# 3 Nonfunctional Requirements

## 3.1 Operational Requirements

Usability: 95% of users will not need to read the user manual to be able to use the application.

## 3.2 Performance Requirements

Maintainability: Changes made to the Manage My ID website can be adopted without altering the iOS application.

## 3.3 Security Requirements

The Roo Balance app has two features.  For the first feature, Use Case 1, Roo Bucks account security is provided by secure login to the managemyid website.  Login information input via the Roo Balance app will not be stored.  For the second feature, Use Case 2, no security is required and access to Roo Bucks locations is available to all users.

## 3.4 Documentation and Training

The Roo Balance application will be delivered to users as a download without documentation or training.  A user guide and system documentation will be provided to project stakeholders.

## 3.5 External Interface

### 3.5.1 User Interface

The user interface will be eye-catching and visually appealing.  When users access their Roo Bucks accounts, the interface will provide a smooth transition with the Manage My ID website which has a straightforward, understated look and feel.

The interface will be intuitive.  As a mobile app it will be streamlined and simple to use.  No training will be provided and it is expected that 95% of users will be able to use the app without any training.

### 3.5.2 Software Interface

The Roo Balance proxy server will serve as an interface between the iOS application and Manage My ID website.  It will enable interaction between the user and the remote website.

# 4 Functional Requirements

## 4.1 Required Features

### 4.1.1 Use Case: 1

Description: User Login / Check Roo Bucks Balance

Actors: student or any Roo Bucks user

Value = high

Cost = high

Basic Path

1. User clicks icon for Roo Bucks application.
2. System prompts user to select an option: View Account or View Locations.
3. User clicks View Account option.
4. System prompts user to enter user e-mail and password.
5. User enters correct user e-mail and password and clicks Login.
6. System displays Account Summary with Roo Bucks balance with options to logoff or view transactions.
7. User clicks Logoff.
8. System exits.

Alternate Path

1. User clicks icon for Roo Bucks application.
2. System prompts user to select an option: View Account or View Locations.
3. User clicks View Account option.
4. System prompts user to enter user e-mail and password.
5. User enters incorrect user e-mail and/or password and clicks Login.
6. System displays error message: &quot;Invalid Email Address and / or Password for user@wrongaddress.com ..... Or you may have exceeded the number of consecutive attempts allowed. Please try again later.&quot;
7. User may choose to login again, returning to step 1, or exit.
8. System exits.

### 4.1.2 Use Case: 2

Description: Find Where to Spend Roo Bucks

Actors: student or any Roo Bucks user

Value = high

Cost = medium

Basic Path

1. User clicks icon for Roo Bucks application.
2. System prompts user to select an option: View Account or View Locations.
3. User clicks  View Locations option.
4. System displays Roo Bucks locations, possibly on more than one screen, with an exit option.
5. User clicks exit.
6. System exits.

## 4.2 Optional Features

### 4.2.1 Use Case: 3

Description: Check Roo Bucks Recent Transactions

Actors: student or any Roo Bucks user

Value = medium

Cost = high

Basic Path

1. Following Login [Use Case 1 Step 6]: System displays Account Summary with Roo Bucks balance with options to logoff or view transactions.
2. User clicks View Transactions.
3. System displays recent transactions with option to logoff.
4. User clicks Logoff.
5. System exits.
