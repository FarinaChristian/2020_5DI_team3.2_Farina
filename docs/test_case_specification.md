# Test Case Specification

**TEAM 4**

Genuary 15, 2020

Prepared by:

Campagnola Jacopo	Farina Christian	Hinegk Giorgio	Pertile Gian Marco

# Table of Contents

1 Introduction 

2 Test Cases: iOS Application 

3 Test Cases: Proxy Server 

Revision History

| Version | Date     | Name                                                         | Description                                                 |
| ------- | -------- | ------------------------------------------------------------ | ----------------------------------------------------------- |
| 1       | 11/07/19 | Campagnola Jacopo, Farina Christian, Hinegk Giorgio, Pertile Gian Marco | Initial Document                                            |
| 2       | 12/11/19 | Campagnola Jacopo, Farina Christian, Hinegk Giorgio, Pertile Gian Marco | Updated test case numbers to eliminate typographical errors |

# Introduction

This document provides the test cases to be performed for the SF-Agriculture application. Each item to be tested is represented by a single test case. Each case describes in detail the expected input and outputs.

# Test Cases: iOS Application

| Test ID          | 2.1                                                          |
| ---------------- | ------------------------------------------------------------ |
| Title            | Correct Login                                                |
| Feature          | Login to www.SF-Agriculture.com with SF-Agriculture App      |
| Objective        | Confirm that proper user id an password yields access to the website as expected. |
| Test Actions     | 1. Start SF-Agriculture application  2. Select View Account option  3. Enter login information |
| Expected Results | System displays account balance with option to logoff.       |

| Test ID          | 2.2                                                          |
| ---------------- | ------------------------------------------------------------ |
| Title            | Incorrect Password                                           |
| Feature          | Login to www.SF-Agriculture.com with SF-Agriculture App      |
| Objective        | Confirm that valid user id with an invalid password denies access to the website without leaving the user stranded. |
| Test Actions     | Start SF-Agriculture application. Select View Account option3. Enter invalid login information |
| Expected Results | System displays error message with option to try again.      |

| Test ID          | 2.3                                                          |
| ---------------- | ------------------------------------------------------------ |
| Title            | Incorrect User E-Mail                                        |
| Feature          | Login to www.SF-Agriculture.com with SF-Agriculture App      |
| Objective        | Confirm that invalid user id denies access to the website without leaving the user stranded. |
| Test Actions     | 1. Start SF-Agriculture application  2. Select View Account option  3. Enter invalid login information |
| Expected Results | System displays error message with option to try again.      |

| Test ID          | 2.4                                                          |
| ---------------- | ------------------------------------------------------------ |
| Title            | Select Option View Locations                                 |
| Feature          | Display merchant locations accepting SF-Agriculture.         |
| Objective        | Confirm that a list of locations is displayed after the user selects the option. |
| Test Actions     | 1. Start SF-Agriculture application  2. Select View Locations option |
| Expected Results | System displays list of merchants with addresses.            |

| Test ID          | 2.5                                                          |
| ---------------- | ------------------------------------------------------------ |
| Title            | Select Option View Transactions                              |
| Feature          | Display recent SF-Agriculture account transactions.          |
| Objective        | Confirm that recent transactions are displayed properly.     |
| Test Actions     | 1. Start SF-Agriculture application  2. Select View Account option  3. Select View Transactions option |
| Expected Results | System displays recent transactions legibly with option to log-off. |

# Test Cases: Proxy Server

| Test ID          | 3.1                                                          |
| ---------------- | ------------------------------------------------------------ |
| Title            | Correct Login                                                |
| Feature          | Login to www.SF-Agriculture.com via proxy server             |
| Objective        | Confirm that proper user id an password yields access to the website as expected. |
| Test Actions     | 1. Go to proxy server http site defined in setup.  2. Enter correct login information3. Press submit |
| Expected Results | Site displays numeric balance for account.                   |

| Test ID          | 3.2                                                          |
| ---------------- | ------------------------------------------------------------ |
| Title            | Incorrect Password                                           |
| Feature          | Login to www.SF-Agriculture.com via proxy server             |
| Objective        | Confirm that invalid password denies access to the website and returns an error. |
| Test Actions     | 1. Go to proxy server http site defined in setup.  2. Enter login information as defined in test data  3. Press submit  4. View page source. |
| Expected Results | Error tag is evident in page source.                         |

| Test ID          | 3.3                                                          |
| ---------------- | ------------------------------------------------------------ |
| Title            | Incorrect User E-Mail Login                                  |
| Feature          | Login to www.SF-Agriculture.com via proxy server             |
| Objective        | Confirm that invalid user id denies access to the website and returns an error. |
| Test Actions     | 1. Go to proxy server http site defined in setup.  2. Enter login information as defined in test data  3. Press submit  4.View page source. |
| Expected Results | Error tag is evident in page source.                         |

| Test ID          | 3.4                                                          |
| ---------------- | ------------------------------------------------------------ |
| Title            | View Transactions via Proxy Server                           |
| Feature          | View transaction history on www.SF-Agriculture.com via proxy server |
| Objective        | Confirm that transaction history is accessed and retrieved from the website correctly. |
| Test Actions     | 1. Go to proxy server http site defined in setup.  2. Enter login information as defined in test data  3. Press submit  4. View page source. |
| Expected Results | Recent transactions are displayed and numbers match those on        www.SF-Agriculture.com. |

