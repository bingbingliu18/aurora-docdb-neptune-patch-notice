# REST API for Amazon DocumentDB

## Introduction
Periodically, Amazon DocumentDB, Aurora, and Neptune perform maintenance on resources. Maintenance most often involves updates to the DB cluster's underlying hardware, operating system (OS), or database engine version. It is necessary to apply database patches in a timely manner and update the OS or database engine version to better protect your cloud database.

In this project, we introduce a serverless solution to get notification when a required patch is scheduled for your cluster. 

This project contains a SAM template and source
code for the primary Lambda functions.

### Inputs
The following are the inputs to the SAM template:
- EmailAddress for receiving email


## Build
To validate the SAM template run:

```
sam validate
```

To build the SAM template run:

```
sam build
```

or 

```
make build
```

## Deploy
To deploy, run

```
sam deploy --capabilities CAPABILITY_NAMED_IAM --guided
```

or 

```
make sam
```

==============================================

Copyright 2020 Amazon.com, Inc. or its affiliates. All Rights Reserved.

SPDX-License-Identifier: MIT-0

