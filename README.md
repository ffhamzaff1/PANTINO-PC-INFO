Act as a senior C#/.NET 8 developer and software deployment engineer.

I have a Windows desktop application called **PantinoPcInfo**, built with C# and .NET 8 for Windows. I publish it using Visual Studio with Release configuration, `win-x64`, and `Self-contained`.

My website has a strict upload limit of **10 MB**, but my published executable is too large to upload.

Your task is to analyze my existing project and implement the best safe solution.

### Requirements

1. Analyze the project structure, `.csproj`, dependencies, resources, images, and published output to identify what makes the application large.
2. Reduce the executable size as much as reasonably possible without breaking existing features.
3. Enable and correctly configure single-file publishing, trimming only if it is safe, and other appropriate .NET 8 publishing optimizations.
4. Preserve all existing functionality, UI, database operations, configuration files, and required resources.
5. Do not delete essential dependencies, database files, or application features just to reduce the file size.
6. Ensure the application can run on other compatible Windows x64 computers, including computers without the .NET Runtime installed, if a self-contained build is used.
7. If the complete self-contained application cannot reasonably fit under 10 MB, do not artificially damage the application. Instead, create a reliable publishing solution that packages the application into a ZIP archive or installer, or hosts the complete release externally and provides a download link for my website.
8. Verify the published output and test the application after making changes.
9. Check for hardcoded local file paths, missing dependencies, and database paths that could prevent the application from working on other computers.
10. Do not expose database passwords, API keys, or other secrets in the published files.

### Important instructions

- Inspect the existing code before changing anything.
- Make a backup before modifying project configuration.
- Do not rewrite the application from scratch.
- Do not claim that the problem is fixed unless you have verified the result.
- Explain every important change and provide the exact publishing commands and settings.
- Keep the solution compatible with .NET 8 and Windows x64.

**Final objective:** Deliver a smaller, reliable, distributable version of PantinoPcInfo that can be downloaded from my website and installed or launched on other compatible Windows PCs. If a file smaller than 10 MB is not technically feasible, implement the best alternative without sacrificing application functionality.
