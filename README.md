# WASOC Workbooks - How to deploy the workbooks into an Azure Sentinel Workspace
This process is for the _manual_ deployment of **Azure Workbooks** to an Azure Sentinel workspace. This will allow for workbooks to appear in the workbook gallery.


## Step-1: Copy the code from WASOCWorkbooks
WASOC workbooks are located in [wagov/WASOCWorkbooks](https://github.com/wagov/WASOCWorkbooks) repository.
Locate the workbooks you want in the GitHub Repo. Click the "Raw" button on the page to "sanitize" the code. Sanitizing code ensures there's no hidden characters or bad formatting.
We use **WASOC - Threat Hunting - Rapid IoC Search.json** as example.

![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/cb6582ff-be27-4a17-bd1f-ca0cae650414)
![Sanitize the code](https://github.com/wagov/WASOCWorkbooks/assets/43643214/a8ea0825-5266-4290-b8b9-09ea8ccd2954)

## Step-2: Navigate to Azure Sentinel | Workbooks

Navigate to your Microsoft Sentinel console, select **Workbooks** in the side blade, and choose the "_Add workbook_" 
![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/ad2ae6ea-22eb-4135-aea6-b6c335c5ea18)

<br>

Once the sample workbook displays, select _Edit_ mode,
![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/73bbb56c-94a2-4d1d-922a-faed864f247b)

<br>

Then choose the Advanced editor (</>) icon.
![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/5a800d21-e0eb-438c-abc5-ab5d10d0a3a9)

## Step-3: Copy / Paste / Apply
Copy the Workbook code from the GitHub repository as raw format,
![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/f5c58b76-df26-4b5f-acc7-7a3caa85a750)

<br>

Once the code has been copied, replace ALL the sample code in the _Gallery Template_ space with the code you copied from the GitHub repo, then, click the **_Apply_** button.
![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/bbb11b65-c977-4f46-afba-7d5f55187b3d)


## Step-4: Name it and Save it
When you applied the code change, the new Workbook will display. Finialise changes by clicking the Save (diskette) icon, and give the Workbook a unique name.

![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/4f21bd14-cd84-4c90-994e-62ffadc70555)

<br>

Note: the **Subscription** and **Resource group** must be the **same** with your Microsoft Sentinel instance **location**, to be accessible from Workbooks Gallery in Sentinel.

![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/2c16665d-792a-47ed-82b3-9c0157f20217)

Click the **_Apply_** button, the workbook has now been deployed
