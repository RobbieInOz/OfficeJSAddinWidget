# Sample code for the Web Widget that promote the Office add-in.

The webpage will show the add-in name, a few details about the add-in functionality for highlight, a dropdown button to install and use the add-in and an image to demo the add-in. This is what the UI looks like.

<img alt="DemoUI.png" src="https://github.com/OfficeDev/OfficeJSAddinWidget/blob/main/Example-ScriptLab-UI.png">

> [!IMPORTANT]  
> To use this sample code, please follow the [Partner-Led Marketing Guidelines](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fforms.office.com%2Fpages%2Fresponsepage.aspx%3Fid%3Dv4j5cvGGr0GRqy180BHbR9SZm6iKPzNJvudw-PPFJydUNFZOMTJVWlVaOTRHQVQ5RENQMUEwWVdaMC4u&data=05%7C02%7Camha%40microsoft.com%7C65489391094a4ceb72fe08dc488e5159%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C638465023522998462%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=vVQh3Binli51i8S8T81j%2F4b9%2F0OtDfXYUj1q2HWug1g%3D&reserved=0).

> [!TIP]
> If you want a simple trial on the dropdown button link that enables user to install and use add-in, please clone https://github.com/OfficeDev/OfficeJSAddinWidget/blob/main/LinkGenerator.html to your local, open with browser app and input the information as the UI shows.

## Usage

1. Download the Example-ScriptLab.html file and go to <script> at line 62.

2. Config the paramenters under "Paramenters that need to config" part.<br>
	a. <strong>addinId</strong><br>
		This is the unique add-in ID. You can get the correct value by following below steps.<br>
		&emsp;1) Go to https://appsource.microsoft.com/en-US/ from your browser.<br>
		&emsp;2) Input your Office add-in name in the search bar on top center of AppSource homepage.<br>
		&emsp;3) Click your add-in in the seach results.<br>
		&emsp;4) The add-in information page will be automatically displayed in current tab.<br>
		&emsp;5) The add-in ID is in the URL.<br>
   For example, if the URL is https://appsource.microsoft.com/en-US/product/office/WA104380862?tab=Overview, then "WA104380862" is the add-in ID that you should input for this parameter in sample code.
		
	b. <strong>addinName</strong><br>
		This is the add-in name. You can get the correct value by following below steps.<br>
		&emsp;1) Go to the webpage in 2.a.4).<br>
		&emsp;2) The add-in name is displayed as the title on right of the add-in icon.<br>
   For example, if the webpage is https://appsource.microsoft.com/en-US/product/office/WA104380862?tab=Overview, then "Script Lab, a Microsoft Garage project" is the add-in ID that you should input for this parameter in sample code.
		
	c. <strong>wordOnlineSupported, excelOnlineSupported, powerpointOnlineSupported, desktopSupported</strong><br>
		This is the Office products that this add-in supports. You can get the correct value by following below steps.<br>
		&emsp;1) Go to the webpage in 2.a.4).<br>
		&emsp;2) Click "details + support" tab on the webpage.<br>
		&emsp;3) Scroll down to "Products supported" section.<br>
			&emsp;&emsp;- If "Word on the web" is in the list, then set wordOnlineSupported to true. Otherwise, set it to false.<br>
			&emsp;&emsp;- If "Excel on the web" is in the list, then set excelOnlineSupported to true. Otherwise, set it to false.<br>
			&emsp;&emsp;- If "PowerPoint on the web" is in the list, then set powerpointOnlineSupported to true. Otherwise, set it to false.<br>
			&emsp;&emsp;- If any item contains "Windows" or "Mac", then set desktopSupported to true. Otherwise, set it to false.<br>
			
	d. <strong>addinDetails</strong><br>
		This is for descriptions about the add-in functionalities displayed on the webpage. 
		
	e. <strong>demoImage</strong><br>
		This is the image for the add-in that display on the webpage.
		
4. Save the html file and open by browser. Verify the UI and dropdown links works for your scenario.

5. Make any additional changes to the sample code as you need, and integrete it into your website.

## Special Notice

The deeplink can successfully open an Office document with your add-in and the end users can use your add-in for below scenarios only.

1. The add-in is public published, so that it can be found from Office AppSource https://appsource.microsoft.com/.

2. The Office store is enabled for the end user.




## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
