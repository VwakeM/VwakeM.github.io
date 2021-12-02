---
title: 'Deploying Shiny Apps to Google Cloud Run'
date: 2022-01-01
permalink: /deploy-rshiny-to-cloudrun
tags:
  - cool posts
  - category1
  - category2
---

RStudio's Shiny library provides is a great option for building interactive web applications and dashboards in R. In this blog post, I will share how you can deploy Shiny applications to Google Cloud Platform's Cloud Run. This is an attractive option if your are using GCP as a cloud provider within your organisation. 

The main steps: 

1. Dockerize your Shiny app. 
2. Create a trigger in Cloud Build. 
3. Create a service in Cloud Run.

1. Dockerize your Shiny application. 
a) Reorganize your folder structure to:
  Root
  |---www
  |Dockerfile
  |shiny-server.sh
  
2. Create a trigger in Cloud Build. 
Automatic invocations are better.

3. Create a service in Cloud Run. 
Options for authenticated or non-authenticated invocations. 
