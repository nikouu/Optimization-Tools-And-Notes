# Optimization Tools And Notes
Tools and notes for C#/.NET optimization. Whether it's size or speed. 

This is different from my [dotnet-optimization-cheatsheet](https://github.com/nikouu/dotnet-optimization-cheatsheet) repo as that is mostly code tricks for performance, and this is mostly tools to help understand and make performance better.

Want to see how Microsoft does it? Check out their [documentation for profiling dotnet/runtime](https://github.com/dotnet/performance/blob/main/docs/profiling-workflow-dotnet-runtime.md).

## Visual Studio Profiler

Built-in code profiler for Visual Studio

[Official Docs](https://learn.microsoft.com/en-us/visualstudio/profiling/profiling-feature-tour?view=vs-2022)
[Reducing Compute Costs Docs](https://learn.microsoft.com/en-us/visualstudio/profiling/optimize-code-using-profiling-tools?view=vs-2022)

## ILSpy

.NET Decompiler

[GitHub Repo](https://github.com/icsharpcode/ILSpy)

## Sizoscope

.NET tool to analyze size of Native AOT binaries

[GitHub Repo](https://github.com/MichalStrehovsky/sizoscope)

## SharpLab

.NET language playground. See decompiled code on the fly in-browser

[SharpLab.io](https://sharplab.io/)

## BenchmarkDotNet

Powerful .NET library for benchmarking

[Official Site](https://benchmarkdotnet.org/)

[GitHub Repo](https://github.com/dotnet/BenchmarkDotNet)

## DependencyGraphViewer

See what methods are kept after AOT trimming

[GitHub Repo](https://github.com/dotnet/runtime/tree/main/src/coreclr/tools/aot/DependencyGraphViewer)

## DUMPBIN

See what is inside a DLL (or other binary files)
```
dumpbin /EXPORTS C:\Windows\System32\msvcr120.dll > C:\Temp\dump.txt
```
[Official Docs](https://learn.microsoft.com/en-us/previous-versions/visualstudio/visual-studio-2008/c1h23y6c(v=vs.90))

## Ildasm

Old school ILSpy

```
ildasm binary.dll
// or
ildasm binary.exe
```
[Official Docs](https://learn.microsoft.com/en-us/dotnet/framework/tools/ildasm-exe-il-disassembler)

## Disasmo

Visual Studio extension to disassemble methods or classes. Similar to IlLSpy but in Visual Studio.

[Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=EgorBogatov.Disasmo)
[Disasmo GitHub](https://github.com/EgorBo/Disasmo)

## DotNet Performance Lab Results

The results of [dotnet/performance](https://github.com/dotnet/performance) runs to check for regressions: [Lab Reports](https://pvscmdupload.blob.core.windows.net/reports/allTestHistory/TestHistoryIndexIndex.html)
