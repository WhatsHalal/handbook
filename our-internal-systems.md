# Our Internal Systems

Besides the customer-facing applications, like the different versions of WhatsHalal, we have a number of internal systems that help us support, report, and operate the company. They are as follows:

### Merchant Management System (MMS)

The MMS is what we use to onboard and manage merchants. This is where we control the merchant opening times, menus and orders.

https://mms.whatshalal.com/


### Delivery Management System (DMS)

The DMS is what we use to onboard and manage delivery partners. Controllers, Operators, Storemen and Execs will utilise this system most of the time.

https://dms.whatshalal.com/


### Sentry

We track programming exceptions on Sentry. When a customer hits a "Oops, something went wrong!" screen, that means there'll be an entry in Sentry explaining to programmers why they saw that screen. Keeping the exceptions under control and monitored is primarily the responsibility of SIP and Jim via on-call.

https://getsentry.com/


### Shipshape

Shipshape is how we make sure our Golang source code are up to WhatsHalal's strict security protocol. Shipshape is a static program analysis platform that allows custom analyzers to plug in through a common interface. Shipshape is packaged in a docker image. When that image is run, a Shipshape analyzer service starts up and processes analysis requests. Structured analysis results are generated. Shipshape can be run as a command-line interface, or as a Jenkins plugin. The requirements to run are that you are running Linux with docker installed and the source code you want to analyze available on disk.

https://github.com/whatshalal/shipshape


### Brakeman

Brakeman is how we make sure our Ruby source code are up to WhatsHalal's strict security protocol. Brakeman is an open source vulnerability scanner specifically designed for Ruby on Rails applications. It statically analyzes Rails application code to find security issues at any stage of development.

https://github.com/whatshalal/brakeman
