# Citrix-Virtual-Apps-and-Desktops-V4
Script to document Citrix Virtual Apps and Desktops, minimum version 2603

Creates an inventory of a Citrix Virtual Apps and Desktops (CVAD) 2603 or later Site using Microsoft PowerShell, Word, plain text, or HTML.

This script requires at least PowerShell version 5.

Default output is now HTML.

You do NOT have to run this script on a Controller. This script was developed and run from a Windows 11 VM.

You can run this script remotely using the –AdminAddress (AA) parameter.

This script supports versions of CVAD starting with 2603.

If you are running XA/XD 7.0 through 7.7, please use: 
https://carlwebster.com/downloads/download-info/xenappxendesktop-7-x-documentation-script/

If you are running XA/XD 7.8 through CVAD 2006, please use:
https://carlwebster.com/downloads/download-info/xenappxendesktop-7-8/

If you are running CVAD 2006 through 2511, please use:
https://github.com/CarlWebster/Citrix-Virtual-Apps-and-Desktops-V3

If you are running Citrix Cloud, please use:
https://carlwebster.com/downloads/download-info/citrix-cloud-citrix-virtual-apps-and-desktops-service/

NOTE: The account used to run this script must have at least Read access to the SQL Server(s) that hold(s) the Citrix Site, Monitoring, and Logging databases.

By default, only gives summary information for:\
&emsp;Administrators\
&emsp;App-V Publishing\
&emsp;Application Groups\
&emsp;Applications\
&emsp;Controllers\
&emsp;Delivery Groups\
&emsp;Hosting\
&emsp;Logging\
&emsp;Machine Catalogs\
&emsp;Policies\
&emsp;StoreFront\
&emsp;Zones

The Summary information is what is shown in the top half of Citrix Web Studio for:
	Machine Catalogs\
	Delivery Groups\
	Applications\
	Policies\
	Logging\
	Controllers\
	Administrators\
	Hosting\
	StoreFront

Using the MachineCatalogs parameter can cause the report to take a very long time to complete and can generate an extremely long report.

Using the DeliveryGroups parameter can cause the report to take a very long time to complete and can generate an extremely long report.

Using both the MachineCatalogs and DeliveryGroups parameters can cause the report to take an extremely long time to complete and generate an exceptionally long report.

Using BrokerRegistryKeys requires the script runs elevated.

Creates an output file named after the CVAD Site.

Word and PDF Document includes a Cover Page, Table of Contents and Footer.

Includes support for the following language versions of Microsoft Word:
	Catalan\
	Chinese\
	Danish\
	Dutch\
	English\
	Finnish\
	French\
	German\
	Norwegian\
	Portuguese\
	Spanish\
	Swedish
