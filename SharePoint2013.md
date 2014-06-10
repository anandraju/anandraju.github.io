# SharePoint 2013

set PreReqPath="E:\Install\SharePoint\PrerequisiteInstallerFiles"
PrerequisiteInstaller.exe /SQLNCli:%PreReqPath%\sqlncli.msi ^
	/PowerShell:%PreReqPath%\Windows6.1-KB2506143-x64.msu ^
	/NETFX:%PreReqPath%\dotNetFx45_Full_x86_x64.exe ^
	/IDFX:%PreReqPath%\Windows6.1-KB974405-x64.msu ^
	/Sync:%PreReqPath%\Synchronization.msi ^
	/AppFabric:%PreReqPath%\WindowsServerAppFabricSetup_x64.exe ^
	/IDFX11:%PreReqPath%\MicrosoftIdentityExtensions-64.msi ^
	/MSIPCClient:%PreReqPath%\setup_msipc_x64.msi ^
	/WCFDataServices:%PreReqPath%\WcfDataServices.exe ^
	/KB2671763:%PreReqPath%\AppFabric1.1-RTM-KB2671763-x64-ENU.exe	
