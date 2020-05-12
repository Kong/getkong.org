---
title: Kong Enterprise 1.5.x Release Notes
---

These release notes apply to Kong Enterprise Release 1.5.x and include information about new features and updates. For detailed information about this release, including features and fixes, see the [_Changelog_](https://docs.konghq.com/enterprise/changelog//).

## New Features

### Consumer Alerts in Kong Immunity 
Kong Immunity detects service behavior anomalies using machine learning. This release extends this functionality with detection of anomalies scoped to specific API consumers. This means all existing triggered alerts now come in two flavors:
* endpoint alerts based on traffic belonging to a specific endpoint
* consumer alerts based on traffic in a workspace for a specific consumer 
With consumer alerts functionality, alerts can now be specifically traced to individuals and teams that access APIs. We’ve also made a few improvements to services and routes pages in Kong Manager to account for these alerts. See [_Immunity Alerts_](https://docs.konghq.com/enterprise/1.5.x/brain-immunity/alerts/). 

### OpenID Connect Improvements
The OpenID Connect plugin bundled with Kong Enterprise 1.5.x features several improvements and fixes. The biggest addition is support for assertions on client authentication. The plugin is now able to authenticate itself with the OpenID Connect Providers using `client_secret_jwt` and `private_key_jwt` authentication methods. See [_OpenID Connect_](https://docs.konghq.com/hub/kong-inc/openid-connect/). 

### Application Registration [_Beta_](https://docs.konghq.com/enterprise/latest/introduction/key-concepts/#beta) 
The ability for developers to create applications that package together a set of backend services is enabled through the Developer Portal and Kong Manager. The Developer Portal includes a new tab called “My Apps” that allows developers to create new applications (and credentials) and subscribe their applications to specific services/APIs. A new “Portal Application Registration” plugin is available, and added functionality in Kong Manager to provide API owners the ability to approve application access to underlying services.

This feature is currently designated as [_beta_](https://docs.konghq.com/enterprise/latest/introduction/key-concepts/#beta). For beta features, we provide full support only in pre-production environments. See [_Application Registration_](https://docs.konghq.com/enterprise/1.5.x/developer-portal/administration/application-registration/).

## Other Improvements
Apart from the highlighted features mentioned above, this version of Kong Enterprise includes several smaller features, including:
* Full support for storing sensitive data fields in an encrypted format at rest within the database
* Sortable entity lists in Kong Manager
* Auto-detection of Apache Cassandra cluster topology without Kong restarts
* A new hostname attribute for upstreams
* IPv6 support for the IP Restriction plugin
* Several other plugin improvements and bug fixes as defined in the Changelog.

## New or Updated in the Documentation

New or updated features in the user documentation include:

* Getting Started Guide walks you through Kong concepts and foundational API gateway features and capabilities.
* Introduction to Kong Enterprise gives an overview of features and architecture. 
* Key Concepts and Terminology defines concepts and terms specific to Kong Enterprise.
* Default Ports list. 
* Kong Security Update Process includes information about reporting a vulnerability and fix development process. 
* Resource Sizing Guidelines is now located in the Deployment section.
* Upgrade and Migration Steps for 1.5. 
* Kong Brain and Kong Immunity: 
** Overview diagram
** Setting Up Collector App via Helm
* New Doc Site updates, including:
** New look and layout
** New Introduction and Deployment sections
** Left navigation, with collapsable sections
** On this page navigation for each topic
** Expanded Search bar
** Tabs in sections, for features such as Kong Manager and Admin API information

## Changelog
For a complete list of changes, please see the Kong Enterprise 1.5.x [_Changelog_](https://docs.konghq.com/enterprise/changelog//).