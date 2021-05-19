# Assessment Aggregations Process API

# Project Description
The Assessment Aggregation API app is a process level api that allows users to get the average of assessment scores by assessment type and category data. It connects to the Category Service API and the Assessment Service API, which encapsulate data from the Caliber API.

# BUILT WITH
- Mulesoft 
- MUnit 
- Log4J
- Maven
- Anypoint Platform
- Anypoint Studio
- REST
- Git
- AWS

# GETTING STARTED
- Go to ${users.home}/m2 folder:
- Rename or delete repository
- Rename settings.xml
- git clone https://github.com/Caliber-Mulesoft/assessment-aggregations-papi.git
- Import project qc-system-api into Anypoint Studio (the folder containing the project has the same name).
- Deploy to CloudHub (Anypoint Platform)
- Please refer to the SETUP document for more detailed installation steps.
  
# PREREQUISITES
- Anypoint platform
- Anypoint studio 7.8.0
- OpenJDK 8
- Embedded Maven
- HTTP connector 1.5.24
- APIkit 1.5.1

# ENVIRONMENT VARIABLES
N/A

# USAGE EXAMPLES
Get the average of assessments by category: /category/average: 

Example response:
```
[
  {
    "category": "SOAP",
    "aggregatedScore": 76.54
  },
  {
    "category": "REST",
    "aggregatedScore": 87.65
  }
]
```

Get the average of assessments by type: /type/average:

Example response:
```
[
  {
    "assessmentType": "Written Evaluation",
    "aggregatedScore": 89.65
  },
  {
    "assessmentType": "Oral Exam",
    "aggregatedScore": 76.25
  }
]
```

# ROADMAP
  <!--Include a list of bugs/issues and possible future fixes here. 
      Don't fill this out until we reach code freeze or if you are ready to deploy.-->

# ADDITIONAL MATERIAL
  <!-- Include a list of any additional materials, like external 
    libraries or resources that must be manually added to run the project, if any. -->

# AUTHORS
Christopher Proutt
