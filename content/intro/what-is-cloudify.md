---
layout: bt_wiki
title: What Is Cloudify?
category: Intro
draft: false
weight: 100

---

Cloudify is an open source cloud orchestration framework that allows you to model applications and services and automate their entire life cycle on the cloud. It lets you deploy on any cloud or data center environment, monitoring all aspects of the deployed application. Failures and other issues are detected and remediated automatically, but manual intervention is always an option.  On-going maintenance tasks are automated, freeing your team for creative and productive activities.


# Application Orchestration

Your application in its entirety (Infrastructure, Middleware, Application Code, Scripts, Tool Configuration, Metrics and Logs) can be described in a Blueprint.
Written in a human-readable YAML format, blueprints allow your applications to be configured in the high granularity for which they were intended.

You can define the complete lifecycle of each part of your application in a blueprint. Cloudify  deploys and manages your applications using the tools you have chosen for each one of them.

As Cloudify launches compute instances, it configures the network, storage and security infrastructure resources required by your application.
Then it executes scripts or invokes configuration management tools that configure your servers and deploy your middleware and code. (Scripts are executed remotely via SSH or locally.)

# Application Maintenance

Cloudify’s custom workflows make it simple to change your application’s structure.

Cloudify provides metrics and log collection capabilities that stream actionable data to Cloudify.

Cloudify's built-in Data aggregation and visualization allow you to execute a variety of workflows through which either you or Cloudify make informed decisions, both tactical and strategic, based on key business or application performance indicators (KPIs).

Those decisions, in turn, can be configured to enable optional manual triggering or automatic triggering of workflows. On the tactical front, these workflows might include scaling or healing. On the strategic front they may include application behavior analysis workflows, etc.


# Cloudify Plug-ins

Cloudify plug-ins complete the framework.

Cloudify-specific plug-ins can run scripts, CM(??) tools, metrics and logs aggregators, or any other (??) tool for that matter.

A plug-in is an abstraction layer entity that installs, configures and executes a tool or script. Cloudify plug-ins are written in Python, making them coder-friendly.

One Cloudify plug-in example is Cloudify's [Script Plug-in]({{< relref "plugins/script.md" >}}) that lets you map node life cycle operations and workflows to scripts that are included in your blueprint. 

Another Cloudify plug-in, the [Diamond plugin]({{< relref "plugins/diamond.md" >}}), collects system metrics and publishes them to multiple destinations.

Users can write and deploy their own plug-ins and incorporate them into their blueprints.

# Standardization

Cloudify's DSL (Domain Specific Language) is based on [TOSCA](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=tosca) (Topology and Orchestration Specification for Cloud Applications) - an emerging standard led by Oasis.


# Open-Source

Cloudify includes several open-source tools and our Python code which makes coding for Cloudify very coder-friendly.

The main open-source components behind Cloudify are:

* [Nginx](http://nginx.com/)
* [Elasticsearch](https://www.elastic.co/products/elasticsearch)
* [Logstash](https://www.elastic.co/products/logstash)
* [RabbitMQ](http://www.rabbitmq.com/)
* [Riemann](http://riemann.io/)
* [InfluxDB](http://influxdb.com/)
* [Grafana](http://grafana.org/)
* [Flask](http://flask.pocoo.org/)
* [Gunicorn](http://gunicorn.org/)
* [Celery](http://www.celeryproject.org/)
* [Fabric](http://www.fabfile.org/)
* [Diamond](http://diamond.readthedocs.io/)
* [Jinja2](http://jinja.pocoo.org/docs/dev/)

And many more...

Cloudify itself is open-source and accepts contributions.
