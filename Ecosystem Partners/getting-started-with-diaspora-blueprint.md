{{{
  "title": "Getting Started with Diaspora - Blueprint",
  "date": "05-01-2015",
  "author": "<a href='https://twitter.com/KeithResar'>@KeithResar</a>",
  "attachments": [],
  "contentIsHTML": false
}}}



### Description

<img src="//d33np9n32j53g7.cloudfront.net/assets/stacks/diaspora/img/diaspora-stack-110x117-afe5cc13795396f087b0314fc4719909.png" style="border:0;float:right;max-width:250px">

After reading this article, the reader should feel comfortable deploying the Diaspora stack by Bitnami.

<a href="https://bitnami.com/" rel="no-follow">Bitnami</a> has integrated their <a href="https://bitnami.com/stack/diaspora" rel="no-follow">Diaspora stack</a> with the CenturyLink Cloud platform with a single-click deploy solution.  The purpose of this KB article is to help the reader take advantage of this integration to achieve rapid time-to-value for this Diaspora solution.

Diaspora is like having your own, private social network without the privacy and social concerns in large, public social networks. When you run Diaspora, you will create a pod which is part of the decentralized social network. Within Diaspora, you can determine what is visible to friends and family, and what can be seen publicly.


### Audience

CenturyLink Cloud Users


### Deploying Diaspora on a New Server

Diaspora is available as a Blueprint for deployment on a **new server**.

#### Steps


1. **Locate the Blueprint in the Blueprint Library**

  Starting from the CenturyLink Control Panel, navigate to the Blueprints Library. Search for **Diaspora on linux_TITLE** in the keyword search on the right side of the page.

  <!-- TODO - fake tile screenshot -->

2. **Click the Deploy Blueprint button.**

3. **Set Required parameters.**

  Set the following parameters in addition to those associated with your server itself (password, network, group, etc.:

  <!-- TODO - replace with legacy blueprint UI html instead -->

  <div style="margin:1em;color: #838383; background: #f2f2f2; margin:1em; padding: 1em; border:2px solid #e5e5e5;width:500px;">
      <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Site</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="127.0.0.1" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Hostname</div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Service Password</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="***" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Provide service password 6 chars or more</div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Apache server SSL port</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="443" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;"></div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Diaspora site name</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="Site" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Diaspora pod title</div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Username</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Service Username</div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Apache server port</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="80" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;"></div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">User's name</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Users Name</div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Redis port</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="6379" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Redis Server port</div>
    </div>
    <br style="clear:both;">
  </div>

  </div>

5. **Review and Confirm the Blueprint**

6. **Deploy the Blueprint**

  Once verified, click on the `deploy blueprint` button. You will see the deployment details stating the Blueprint is queued for execution.

  This will kick off the Blueprint deploy process and load a page where you can track the deployment progress. Deployment will typically complete within five minutes.

7. **Deployment Complete**

  Once the Blueprint has finished executing on your server you may access Diaspora by navigating to your server via http.


8. **Enable public access** (optional)

  Servers are built using private IPs only with access with client or IPSEC VPN.  For inbound access from the Internet add a public IP to your master server.

  <a href="../../network/how-to-add-public-ip-to-virtual-machine/">
    <img style="border:0;width:50px;vertical-align:middle;" src="../images/shared_assets/fw_icon.png">
    Adding a public IP to your virtual machine
  </a>



### Deploying Diaspora on an existing server (alternate option)

Diaspora is available as a Blueprint Package for deployment on an existing server based on your own sizing requirements or to support more advanced configurations such as customized Blueprint Workflows to repeatably deploy multiple stacks on the same machines

#### Steps


1. **Deploy or Identify an Existing Server**

  Identify the server targeted for Diaspora installation.  Operating sustem must be linux.

  See the [Creating a new enterprise cloud server](../../servers/creating-a-new-enterprise-cloud-server/) KB for more information on completing this step.


2. ** Select to Execute the Package on a Server Group**

  Packages can be executed on one more more servers in a group.  Search for the public script package named **Install Diaspora on linux_TITLE**.

  See the [using group tasks to install scripts on groups](../../servers/using-group-tasks-to-install-software-and-run-scripts-on-groups/) KB for more information on how to complete the next few steps.


3. **Set Parameters**

  Set the following parameters:

  <div style="margin:1em;color: #838383; background: #f2f2f2; margin:1em; padding: 1em; border:2px solid #e5e5e5;width:500px;">
      <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Site</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="127.0.0.1" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Hostname</div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Service Password</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="***" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Provide service password 6 chars or more</div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Apache server SSL port</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="443" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;"></div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Diaspora site name</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="Site" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Diaspora pod title</div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Username</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Service Username</div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Apache server port</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="80" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;"></div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">User's name</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Users Name</div>
    </div>
    <br style="clear:both;">
  </div>

  <div style="padding: 1em;">
    <label style="font-family: 'Open Sans', Helvetica, Arial, Sans-Serif; font-size:14px; margin: 7px 20px 7px 0; padding-top:7px;color:#333333; text-decoration:underline; text-transform:lowercase; float:left; width:160px;text-align:right;">Redis port</label>
    <div style="float:left;margin-left:10px;">
      <input style="padding:4px 6px;width:250px;height:34px;" type="text" value="6379" disabled="disabled">
      <div style="margin-top:10px; color:#999; font-size:13px; line-height:15px;">Redis Server port</div>
    </div>
    <br style="clear:both;">
  </div>

  </div>

4. **Deploy the Blueprint**

  Once verified, click on the `execute package` button. You will see the deployment details stating the Blueprint is queued for execution.

  This will kick off the Blueprint deploy process and load a page where you can track the deployment progress. Deployment will typically complete within five minutes.

5. **Deployment Complete**

  Once the Blueprint has finished executing on your server you may access Diaspora by navigating to your server via http.


6. **Enable public access** (optional)

  Servers are built using private IPs only with access with client or IPSEC VPN.  For inbound access from the Internet add a public IP to your master server.

  <a href="../../network/how-to-add-public-ip-to-virtual-machine/">
    <img style="border:0;width:50px;vertical-align:middle;" src="../images/shared_assets/fw_icon.png">
    Adding a public IP to your virtual machine
  </a>


### Pricing

The costs listed above in the above steps are for the infrastructure only.


### About Bitnami

CenturyLink Cloud works with [Bitnami](http://www.bitnami.com) to provide open source software integrations to its customers.  Bitnami is a library of popular server applications and development environments that can be installed with one click, either in your laptop, in a virtual machine or hosted in the cloud. Bitnami takes care of compiling and configuring the applications and all of their dependencies (third-party libraries, language runtimes, databases) so they work out-of-the-box. The resulting packaged software (a 'stack') is then made available as native installers, virtual machines and cloud images. These Bitnami application packages provide a consistent, secure and optimized end-user experience when deploying any app, on any platform.


### Frequently Asked Questions

**Who should I contact for support?**

* For issues related to cloud infrastructure, please open a ticket using the [CenturyLink Cloud Support Process](../Support/how-do-i-report-a-support-issue.md).
* For issues related to deploying the Bitnami Blueprint on CenturyLink Cloud, Licensing or Accessing the deployed software, please visit the [Bitnami Support website](http://www.bitnami.com/support)

**How do I access Diaspora for the first time?**

Nearly all Bitnami stacks can be accessed and configured by navigating to your server with a web browser.


