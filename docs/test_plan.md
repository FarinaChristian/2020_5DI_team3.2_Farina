Testing Document and Specification

# Test Plan

# SF-Agriculture

 2020

# Introduction

This document outlines the test plan for SF-Agriculture. As indicated in the project requirements document, this system should provide entrepreneurs and staff with a means of asking general health questions. This system will also provide a discussion mechanism between suppliers and students affiliated with suppliers. The testing activities discussed in this document will verify that the software for the question and answer system meets the customer's needs by verifying that the requirements for this system, as indicated in the requirements document, are met.


The test routine will test the answer of the question and answer system when asking a question, browse the questions previously asked, search for questions by keyword, access front-end / back-end websites and publish the answers to the front-end website. The results of this test procedure will allow the creators of this system to evaluate the success of the project, as indicated in the project plan.



# Terminology


The terms user, vendor, system, site and username / password will be frequently used in this document, therefore formal definitions will be provided.

System: the database and bulletin board that supports the website backend

Users: SF-Agriculture affiliates who will only use the website front end

Agricultural entrepreneurs will help oversee and are involved in this website


# Items Tested

Items that will be tested during the testing phase as laid out by the Macro Project Plan will be but are not limited to:



- .Ability for an individual to select a category and read questions/answers pertinent to that category

Test Case: 4.1.4.1, 4.1.4.2

- .Ability for a user to login via username and password 

Test Case: 4.1.1.1, 4.1.2.1, 4.1.2.2, 4.1.2.3

- .Ability for a user to login via username and password and submit a survey

           Test Case: 4.1.3.1

- .Ability for farmers to login via username and password to the back-end system and post answers to the front-end site via a threaded discussion board

Test Case: 4.2.1.1, 4.2.1.2, 4.2.1.3

- .Ability to search (by keyword) through questions and answers

Test Case: 4.1.4.2



# Items Not Tested

There are features that will not be included in the current testing procedure.  This does not mean that these features will not be created, but that they have not been implemented and are not available for testing.  Those features include but are not limited to:

- Input of field data

- Querying the Database

- Functionality for adding and removing a user



# Approach

The general method for this test procedure is manual system testing. Each test case created will have a direct link to the requirements set out in the Requirements Document. Test cases that include similar functionality methods will be tested together. Examples of these features include access to submit a question or access to submit a survey. Test cases like these test the security features of the system together with the ability to send information to the database. Each test case will verify the security functionality with invalid and invalid data (user names and passwords) to ensure that valid user requirements for these features are met.

Features that specify reading the questions asked earlier and searching by keyword will be tested together but in separate test cases. Keyword research through previously verified questions and answers will verify the system's ability to produce results that an individual can visually validate.

Manual system tests will continue throughout the second and third iterations of the project. For each iteration, both old and newly implemented functionality will be tested. The addition of new features or functionality can sometimes interfere with the functionality of old features and to ensure the success of the product, all implemented features should work as expected throughout the life of the software.

# Item Pass/Fail Criteria

The minimum requirements for this software system were laid out in the Requirements Document and the Macro Project Plan outlined what the creators of the software considered project success.

Implemented features that meet the requirements as determined by the customer, meaning the feature does what the user wants it to do with very little difficulty, passes the testing procedure.  Difficulty, as used here, is determined by user comprehension and user ability to use the feature with little to no training.

Features that contain major defects will fail the testing procedure and will be documented via an incident report and turned over to the developer for investigation and revision.

# Test Deliverables

In addition to the test plan, other test results include test specifications that outline the specific test cases and expected results of each test and test reports that include incidents, defects, and changes.

# Testing Tasks

The following list the testing deliverables and the activities required to produce the deliverable.

| Deliverables | Activities |
| --- | --- |
| Test Plan |
- Analyze Requirements for System Features
- Determine Testable and Non-Testable Features
- Develop Approach
- Determine the activity and estimate the costs
- Develop Schedule for Testing
- Analyze Requirements
- Define Test Cases for Testable Features as Outlined by the Test Plan
- Implement Test Cases as Outlined by the Test Specifications
- Document Incidents and Defects
- Determine Severity of Incidents and Defects
- Determine Changes that Need to be Made to System
- Document and Submit Change Request to Developer
  