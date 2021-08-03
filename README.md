# WebcamWinForm

<div align="center">
    <img src="https://gclstorage.blob.core.windows.net/images/WebcamWinForm-banner.png" />
</div>

[![.NET 5 Build](https://github.com/goh-chunlin/WebcamWinForm/actions/workflows/dotnet-5.yml/badge.svg)](https://github.com/goh-chunlin/WebcamWinForm/actions/workflows/dotnet-5.yml)
[![CodeQL](https://github.com/goh-chunlin/WebcamWinForm/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/goh-chunlin/WebcamWinForm/actions/workflows/codeql-analysis.yml)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Donate](https://img.shields.io/badge/$-donate-ff69b4.svg)](https://www.buymeacoffee.com/chunlin)

A simple Windows Forms (.NET 5) application to demonstrate how to record video and audio via a Logitech webcam using C#.

## Objective
In 2017, inspired by ["How to use a web cam in C# with .NET Framework 4.0 and Microsoft Expression Encoder 4", a project on Code Project by Italian software developer Massimo Conti](https://www.codeproject.com/Articles/202464/How-to-use-a-WebCam-in-C-with-the-NET-Framework), I built a simple demo to show how we can connect C# Windows Form with a webcam to record both video and audio.

In 2020, .NET 5 is officially announced by Microsoft. Many libraries that I used earlier are no longer working. Hence, I took the chance to upgraded this project to use .NET 5 together with other new libraries.

The recorded media will be saved as a MP4 file locally. The file will also be uploaded to [Microsoft Azure Storage](https://azure.microsoft.com/en-us/services/storage/) at the same time in a container named "webcam-videos", hence the user interface asks for the connection string to the Azure Storage.

The webcam that I have tested with is [Logitech HD Webcam C270](https://www.logitech.com/en-us/products/webcams/c270-hd-webcam.960-000694.html).

## Important Nuget Packages
- [DirectShowLib.Standard 2.1.0](https://www.nuget.org/packages/DirectShowLib.Standard/);
- [OpenCvSharp4 4.5.0.20201013](https://www.nuget.org/packages/OpenCvSharp4/);
- [OpenCvSharp4.runtime.win 4.5.0.20201013](https://www.nuget.org/packages/OpenCvSharp4.runtime.win/);
- [BasicAudio 2020.11.10.1](https://www.nuget.org/packages/BasicAudio/);
- [FFMpegCore 3.2.4](https://www.nuget.org/packages/FFMpegCore/);
- [Azure.Storage.Blobs 12.7.0](https://www.nuget.org/packages/Azure.Storage.Blobs/).

## License ##

This library is distributed under the GPL-3.0 License found in the [LICENSE](./LICENSE) file.
