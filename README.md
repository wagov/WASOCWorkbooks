# WASOC Workbooks - How to deploy the workbooks into you Azure Sentinel
Deploying code from WASOC GitHub repository to your Azure Sentinel instance is very similar to copy/paste operation. This guidance is specific for **Workbook**


## Step-1: Copy the code from WASOCWorkbooks
WASOC workbooks are located in [wagov/WASOCWorkbooks](https://github.com/wagov/WASOCWorkbooks) repository.
Locate the workbooks you want in the GitHub Repo. Click the "Raw" button on the page to "sanitize" the code. Sanitizing code ensures there's no hidden characters or bad formatting.
We use **WASOC - Threat Hunting - Rapid IoC Search.json** as example.

![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/cb6582ff-be27-4a17-bd1f-ca0cae650414)
![Sanitize the code](https://github.com/wagov/WASOCWorkbooks/assets/43643214/a8ea0825-5266-4290-b8b9-09ea8ccd2954)

## Step-2: Navigate to Azure Sentinel | Workbooks

Navigate to your Microsoft Sentinel console, select **Workbooks** in the side blade, and choose the "_Add workbook_" 
![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/6a67c229-4108-40dc-b712-926f98031e3e)

<br>

Once the sample workbook displays, select _Edit_ mode,
![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/904e1c5c-673f-4f71-b555-72388eb9d89d)

<br>

then choose the Advanced editor (</>) icon.
![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/779bb31f-d226-41e8-8933-18ceecd5b9de)

## Step-3: Copy / Paste / Apply
Copy the Workbook code from the GitHub repo raw,
![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/f5c58b76-df26-4b5f-acc7-7a3caa85a750)

<br>

Once the code has been copied, replace ALL the sample code in the _Gallery Template_ space with the code you copied from the GitHub repo, then, click the **_Apply_** button.
![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/74401503-8cc6-4f41-ab82-f751dea34f9d)


## Step-4: Name it and Save it
When you applied the code change, the new Workbook will display. Finish up by click the Save (diskette) icon, give the Workbook a unique name.

![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/33df471a-6caf-4123-85be-44a22018316b)

<br>

Note: the **Subscription** and **Resource group** must be the same as Microsoft Sentinel, to be accessible from Workbooks Gallery inside Sentinel.

![image](https://github.com/wagov/WASOCWorkbooks/assets/43643214/8d27858d-c819-4ce9-8495-f3cc660fd10e)

Click the **_Apply_** button, the workbook has now been deployed
