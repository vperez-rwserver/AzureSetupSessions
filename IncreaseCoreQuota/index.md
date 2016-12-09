# Request Increase of Core Quota

* On your subscription, click "New support request" at the bottom, then select the following values:
    * Issue Type: **Quota**
    * Quota Type: **Cores**

![Increase quota 1 of 3](https://vperez-rwserver.github.io/AzureSetupSessions/images/increasequota1.png)

* On the Problem blade, select the following values:
    * Deployment model: **Resource Manager**
    * Location: Same location selected for Tableau Server
    * SKU family: Check **A Series** and **D Series**

![Increase quota 2 of 3](https://vperez-rwserver.github.io/AzureSetupSessions/images/increasequota2.png)

* On New quota enter the **Total number of cores needed (already used + extra needed)**

![Increase quota 3 of 3](https://vperez-rwserver.github.io/AzureSetupSessions/images/increasequota3.png)

(**Example**: If "Current quota" says "20" and you are using 8 cores, you need to enter 8+64 = 72 here)

* Fill up Contact options and click Create. Azure support will notify you when your quota has been increased. 

**NOTE**: Some Azure subscriptions such as free trial don't allow increasing core quota. As a workaround you can get a Visual Studio Essentials subscription and [activate its free azure benefit here](https://azure.microsoft.com/en-us/pricing/member-offers/msdn-benefits-details/).
