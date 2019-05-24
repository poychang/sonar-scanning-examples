This example demonstrates how to analyze a .NET Core Solution with the SonarQube Scanner for MSBuild.

Prerequisites
=============
* [SonarQube](http://www.sonarqube.org/downloads/) 5.6+ LTS
* [SonarQube Scanner for MSBuild](http://docs.sonarqube.org/display/SCAN/Analyzing+with+SonarQube+Scanner+for+MSBuild) Core 2.0+
* [SonarSource C# Plugin](http://redirect.sonarsource.com/plugins/csharp.html) 5.5.1+
* [Compatible .NET Build Environment](http://docs.sonarqube.org/display/SCAN/From+the+Command+Line)

Usage
=====
* Run SonarQube Scanner for MSBuild begin phase:

        dotnet <path to SonarScanner.MSBuild.dll> begin /k:"org.sonarqube:sonarqube-scanner-msbuild" /n:"Example of SonarQube Scanner for MSBuild Usage" /v:"1.0"

* Build the project with Dotnet CLI:

        dotnet build <path to solution.sln>

* Run SonarQube Scanner for MSBuild end phase:

        dotnet <path to SonarScanner.MSBuild.dll> end
