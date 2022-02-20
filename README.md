# unoplatform
Learning Uno Platform

https://platform.uno/

***Installing***
It's a pain in the ass this thing!!!!

I had to install VS2019 selecting the workloads:
1. ASP.NET and web development
2. Mobile development with .NET
3. ASP.NET and web development
4. .NET Core cross-platform development

Then, open VS, go to Extensions>Manage Extensions.  Search "uno" and install the one named "Uno Platform solution templates".
Restart VS and a Uno pop-up is open, clic con Manage and wait until it's done.

Then, open command prompt as admin and run
dotnet tool install --global Uno.Check
It throws an error saying that it's already installed.

Then, run
uno-check

It shows a lot of messages and warnings showing pending components to install. 

I had to open VS, go to Tools>Android>SDK Manager and wait until the automatic update was done.

Then go back to the terminal and run uno-check, again errors.  So, I had to install .NET SDK 6.0.100 from here https://dotnet.microsoft.com/en-us/download/dotnet/6.0
Re run uno-check and finally after 20 minutes installing things, I was able to read:

Fix applied.  Checking again...

> .NET SDK - Workloads (6.0.100) Checkup...
  - android-aot (Microsoft.NET.Sdk.Android.Manifest-6.0.100 : 31.0.101-preview.11.81) installed.
  - ios (Microsoft.NET.Sdk.iOS.Manifest-6.0.100 : 15.0.101-preview.11.391) installed.
  - maccatalyst (Microsoft.NET.Sdk.MacCatalyst.Manifest-6.0.100 : 15.0.101-preview.11.391) installed.
  - tvos (Microsoft.NET.Sdk.tvOS.Manifest-6.0.100 : 15.0.101-preview.11.391) installed.
  - macos (Microsoft.NET.Sdk.macOS.Manifest-6.0.100 : 12.0.101-preview.11.391) installed.
  - maui (Microsoft.NET.Sdk.Maui.Manifest-6.0.100 : 6.0.101-preview.10.2068) installed.
─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────

- Congratulations, everything looks great!

Press Enter to finish...


 
