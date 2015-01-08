## Introduction

This repository contains examples for problems when sharing a solution between Xamarin Studio and Visual Studio 2013. This scenario is described here: http://developer.xamarin.com/guides/cross-platform/application_fundamentals/building_cross_platform_applications/part_3_-_setting_up_a_xamarin_cross_platform_solution/

> ... Solutions can be shared across development environments, even when individual projects cannot be loaded (such as a Windows phone project in Xamarin Studio). ...

The problem is that Xamarin Studio and Visual Studio make unexpected changes in the source text of the .sln and .csproj files. These changes are also made back and forth, essentially leading to a commit ping pong between Visual Studio and Xamarin Studio users.

Examples are:

* UUIDs changed from lower to upper case (e.g. SHA: 497b3dfd121a888c8708b541d1590737ef7bef39).
* Reordering of .sln file (e.g. SHA: 497b3dfd121a888c8708b541d1590737ef7bef39).
* Changing the "ToolsVersion" (e.g. SHA: df03210c9211446aba39d9542a0312da50f525e9).
* Changing the "Visual Studio" version (e.g. SHA: df03210c9211446aba39d9542a0312da50f525e9).
* Other changes, like changing line break, changed "true" to "True", ...

## Used tool versions
On Mac OS X 10.10:

* Xamarin Studio, Version 5.5.4 (build 15)
* Xamarin.Android, Version: 4.20.0.28 (Business Edition)
* Xamarin.iOS, Version 8.4.0.47 (Business Edition)
* Mono, Version 3.10.0 ((detached/92c4884)

On Windows 8.1:

* Microsoft Visual Studio Ultimate 2013, Version 12.0.31101.00 Update 4
* Microsoft .NET Framework, Version 4.5.51641
* Xamarin, Version 3.8.150.0
* Xamarin.Android, Version 4.20.0.28
* Xamarin.iOS, Version 8.4.0.0
