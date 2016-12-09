[Home](https://vperez-rwserver.github.io/AzureSetupSessions)

# Tableau and Cloudera

## 1. Spin Tableau Server

1. Click the **+ New** button from the portal, then type "**tableau server**" on the search box and click Tableau Server on the results. 

![1](https://vperez-rwserver.github.io/AzureSetupSessions/images/tableau1.png)

2. Click Create. 

![2](https://vperez-rwserver.github.io/AzureSetupSessions/images/tableau2.png)

3. In the Basics blade enter the following values:
    * Name: **tableauvm**
    * VM disk type: **SSD**
    * User Name: **labuser**
    * Password: **lab@pass1234**
    * Resource group: select **Create new** and type **TableauRG**
    * Location: **\<Location nearest to you\>**

![3](https://vperez-rwserver.github.io/AzureSetupSessions/images/tableau3.png)

4. For virtual machine size, choose DS3 and click Select.

![4](https://vperez-rwserver.github.io/AzureSetupSessions/images/tableau4.png)

5. Leave defaults values on Settings blade, click OK.

6. Review summary and click OK.

7. Click Purchase.

## 2. Ensure prerequisites

Tableau Server will take around 5 minutes to spin up. Let's use this time to ensure prerequisites are configured and neccesary applications are installed:

### Subscription Credit

1. Click on Subscriptions (if not on left menu, click "More services" at the bottom), then double-click at the subscription you will be using for the lab.

2. Find the Burn rate graphic on the Essentials blade, the value under "LEFT TO CAP" is the remaining credit. Must have at least $200 of credit to deploy a small cluster during the lab. 

![5](https://vperez-rwserver.github.io/AzureSetupSessions/images/tableau5.png)

### Core Quota

Follow the steps in [Increase core quota](https://vperez-rwserver.github.io/AzureSetupSessions/IncreaseCoreQuota) to add 64 additional cores to your subscription.

**Note**: If Azure support asks for the reason behind the quota increase, tell them you need the extra cores to deploy a "Cloudera Enterprise Data Hub". 

### Required Software and Drivers

1. Install an ssh client like [putty for windows](https://the.earth.li/~sgtatham/putty/latest/x86/putty-0.67-installer.msi)

2. Install [Cloudera Hive ODBC driver](http://www.cloudera.com/downloads/connectors/hive/odbc/2-5-21.html)

3. Install [Cloudera Impala ODBC driver](http://www.cloudera.com/downloads/connectors/impala/odbc/2-5-36.html)

4. Install [Tableau Desktop](http://www.tableau.com/products/desktop/download)

## 3. Create an Azure SQL Database

TODO

## 4. Create a Cloudera Enterprise Data Hub Cluster

TODO
