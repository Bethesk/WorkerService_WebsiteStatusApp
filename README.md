# WorkerService_WebsiteStatusApp
 Hands-on practice using a Worker Service. 

- The following NuGet packages were added to the project:
  1. Serilog. AspNetCore
  2. Serilog.Sinks.File  (Log events to text files in plain or JSON format)
  3. Microsoft.Extensions.Hosting.WindowsServices
					
					
- Deploying the Windows Service:
  1. Click 'Publish' in Visual Studio
  2. Deploy to a desired folder
				

- Installing the Windows Service
1. Open Powershell as admin
2. Run the following command
   sc.exe  create WebsiteStatus binpath= c:\temp\workerservice\websiteStatus.exe(File Name) start = auto
3. Hit Enter
4. Confirm that the service appears in the Services list
				
- Uninstalling the Window Service
1. Open Powershell as admin
2. Stop the service
   sc.exe stop WebsiteStatus
3. Delete the service
   sc.exe delete WebsiteStatus
   
