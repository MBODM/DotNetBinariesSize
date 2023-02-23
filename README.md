# DotNetMinimumBinarySize
Some simple testing to see how big some compiled .NET binaries are

After a short discussion with a friend of mine (greetings to Stefan), about how much minimal size some different self-contained .NET executables/binaries have (when compiled with "minimum output size" options, like Trimming), i thought it´s a good idea to quickly test this on my own. I just use this GitHub repo to have some place to save the projects and share the results.

So, nothing special here. Just some compiled default Visual Studio 2022 .NET project templates, with all the "minimum binary size" options enabled. The tested project types are:

- .NET 6 CLI Application
- .NET 6 WinForms Application
- .NET 6 WPF Application
- .NET 7 CLI Application
- .NET 7 WinForms Application
- .NET 7 WPF Application

All projects are published as "self-contained" with "win-x64" as target platform. All size options (2 or 3 options), Visual Studio 2022 shows in the Publish UI dialog, were adjusted to "generate smallest executable size".

Results:

- xxx MB (.NET 6 CLI Application)
- xxx MB (.NET 6 WinForms Application)
- xxx MB (.NET 6 WPF Application)
- xxx MB (.NET 7 CLI Application)
- xxx MB (.NET 7 WinForms Application)
- xxx MB (.NET 7 WPF Application)
