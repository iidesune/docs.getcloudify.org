---
layout: bt_wiki
title: Maintenance Mode
category: Manager
draft: false
abstract: Cloudify's Web Interface
weight: 200
---

Managing maintenance mode page will be found at the settings section in the Web UI. Upon routing you will be presented with the manager maintenance mode status and a button used to change it.<br/>
![maintenance mode page]({{< img "ui/maintenance/ui-maintenance-mode-page.png" >}})


Pressing the button to change the maintenance mode status opens a confirmation dialog.<br/>
![confirmation dialog]({{< img "ui/maintenance/ui-maintenance-confirmation-dialog.png" >}})


Confirming makes the manager start entering requested mode, a message will be shown notifying all users.<br/>
![starting maintenance message]({{< img "ui/maintenance/ui-starting-maintenance-message.png" >}})


Once maintenance mode is turned on the Web UI will prevent all actions but turning maintenance mode off.<br/>
![maintenance message]({{< img "ui/maintenance/ui-maintenance-message.png" >}})


The manager will not enter maintenance mode until all running executions are finished. When requesting to turn on maintenance mode while other executions are running, you will be presented with the executions details and an option to cancel each.<br/>
![remaining executions]({{< img "ui/maintenance/ui-maintenance-remaining-executions.png" >}})