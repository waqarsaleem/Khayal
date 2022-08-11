# WASM Comparative Analysis 
## --> C# vs Python :
### 1. Pyodide
Brython’s goal is to replace JavaScript with Python as the scripting language for browsers. A programming alternative to Bryton is Pyodide, which compiles Python 3.9 with a scientific stack to WebAssembly (scientific stack being NumPy, Pandas, SciPy and over 75 packages). It also lets you install pure Python wheels from PyPi. 

### 2. Blazor
If you prefer to program and run C# in the browser, Blazor is the way to go. Like Pyodide, it also appeared in 2018 and comes in two flavors: Server and WebAssembly.  It’s also cross-platform, so you can develop Blazor apps on Linux and Mac as well as Windows. Blazor builds on ASP.NET using Razor syntax which mixes HTML with code

### Conclucion
Each of these programming technologies, including the C# Blazor WebAssembly, uses JavaScript behind the scenes in one way or another, even if only to load a component. But you don’t need to know JavaScript to use any of them.
| **C# ->(Blazor)**                                        | **Python ->(Pyodide)**                                      |
| --------------------------------------------- | ----------------------------------------------- |
| **Overview**                               |
| Blazor lets you build interactive web UIs using C# instead of JavaScript. Blazor apps are composed of reusable web UI components implemented using C#, HTML, and CSS. Both client and server code is written in C#, allowing you to share code and libraries.                          |Pyodide is a Python distribution for the browser and Node.js based on WebAssembly.Pyodide makes it possible to install and run Python packages in the browser with micropip. Any pure Python package with a wheel available on PyPI is supported. Many packages with C extensions have also been ported for use with Pyodide. These include many general-purpose packages such as regex, pyyaml, lxml and scientific Python packages including numpy, pandas, scipy, matplotlib, and scikit-learn.|
| **Platform**                               |
|Blazor is a feature of ASP.NET, the popular web development framework that extends the .NET developer platform with tools and libraries for building web apps. Building interactive web UIs using C# instead of JavaScript. Blazor gives you real .NET running in the browser on WebAssembly.                           |Pyodide comes with a robust Javascript ⟺ Python foreign function interface so that you can freely mix these two languages in your code with minimal friction. This includes full support for error handling (throw an error in one language, catch it in the other), async/await, and much more.When used inside a browser, Python has full access to the Web APIs.            |
| **Libraries**                               |
|Blazor apps can use existing, .NET APIs that are common across all .NET implementations, .NET Standard allows the same code and libraries to be used on the server, in the browser, or anywhere you write .NET code.                            |Pyodide brings the Python runtime to the browser via WebAssembly, along with NumPy, Pandas, Matplotlib, parts of SciPy, and NetworkX.The real power of Pyodide comes from its scientific computing libraries.             |
| **GUIs**                               |
|Get productive fast with re-usable UI components from top component vendors like Telerik, DevExpress, Syncfusion, Radzen, Infragistics, GrapeCity, jQWidgets, and others. Or use one of the many open-source component libraries from the Blazor community.                            |There are not enough GUIs than Blazor. Pyodide Supports mostly Scientific GUIs, which are mentioned above.              |
| **Previous Work**                               |
|Its been a lot of work in this domain such as IOT, Authentication, Cloud, CMS, Logging, Machine Learning, Rapid Development Framework, Build native mobile apps.                            | Worked Specifically in the domain of Data Science.             |
| **Projects**                               |
|A large number of projects are being made                          | lesser number of projects             |
