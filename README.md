# WorkerService_WebsiteStatusApp
 
- Install Nuget Package:
  1. Serilog. AspNetCore
  2. Serilog.Sinks.File  (Log events to text files in plain or JSON format)
  3. Microsoft.Extensions.Hosting.WindowsServices
					
					
- Deploy a window service :
  1. Click 'Publish'
  2. Deploy to a folder
				

- Install a window service
Open Powershell as admin
Run the following command 1. sc.exe  create WebsiteStatus binpath= c:\temp\workerservice\websiteStatus.exe(File Name) start = auto
				        2. Hit Enter
				        3. Notice that a service shows up 
				
- Uninstall a window service 
	1. Stop the service
   2. sc.exe delete WebsiteStatus (Service Name)
   3. Hit Enter
