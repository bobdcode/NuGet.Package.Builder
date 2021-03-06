##Release 1.0.10

 + Added support for excluding wildcard patterns when creating package.
 + Updated NuGet.exe from 2.8.x to 3.3
 + Symbols are new automatically published along with the package on build time.

##Release 1.0.9

 + Fixed issue related to bug fix for 1.0.7 where publishing failed to use the correct package name.

##Release 1.0.8

 + Removed timeout restriction when building and publishing NuGet packages.

##Release 1.0.7

 + Fixed bug where binary output name was used instead of project name when building a nuget package from project.

 + Added support for build configuration specific package generation.

##Release 1.0.6

 + To support generation of packages through nuget.exe pack myproject.csproj a "special" version of 
   NuGet.exe 2.8.5 is included that fixes the issue. see http://nuget.codeplex.com/workitem/4013
   A pull request fixing the issue can be found here https://nuget.codeplex.com/SourceControl/network/forks/StephenCleary/Issue4013/contribution/6798
   It has been merged and will be available in 3.0 so until then the special version will be used.

 + Added support for generating command files for publishing packages at any point after the build process.

##Release 1.0.5

 + Now using NuGet.exe 2.8.5
 + {project}.nuspec files are no longer removed when uninstalling. This fixes the issue with running a Update-Package from Package Manager Console where all .nuspec files will be removed and added again.


##Release 1.0.3

 + Fixed bug when parsing PublishApiKey or PublishSource from MSBuild to NuGet.Package.Builder.
 
 
