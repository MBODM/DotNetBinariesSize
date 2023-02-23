# DotNetMinimumBinarySize
Some simple testing to see how big some compiled .NET binaries are

### What it is

After a short discussion about Rust and Go, with a friend of mine (greetings to Stefan), we thought about how much minimal size some different self-contained .NET executables/binaries may have (when compiled with "minimum output size" options, like Trimming). Therefore i thought it´s a good idea to quickly test this on my own. I just used this GitHub repo to have some place to save the projects and share the results.

So, really nothing special here (translation: _super lame_). 😁

### How it is done

I just opened some default Visual Studio 2022 .NET project templates, enabled all the "minimum output binary size" options in the Publish UI dialog, saved and compiled them. No other changes were made and no code was written. The tested project types are:

- .NET 6 CLI Application
- .NET 6 WinForms Application
- .NET 6 WPF Application
- .NET 7 CLI Application
- .NET 7 WinForms Application
- .NET 7 WPF Application

All projects are published as "self-contained" with "win-x64" as target platform. All size options (2 or 3 options), Visual Studio 2022 shows in the Publish UI dialog, were adjusted to "generate smallest executable size possible". No other "special tricks" (special compiler settings, hidden settings, special optimizations, and so on) were used to further decrease the output binary size (this was done on purpose).

### Results

- xxx MB (.NET 6 CLI Application)
- xxx MB (.NET 6 WinForms Application)
- xxx MB (.NET 6 WPF Application)
- xxx MB (.NET 7 CLI Application)
- xxx MB (.NET 7 WinForms Application)
- xxx MB (.NET 7 WPF Application)
