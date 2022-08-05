# Findings on the descision of tools for building the infrastructure of the Project

Primarliy, the goal of this project is to build a powerful graphing software using WebAssemblies. Hence, we need to choose a primary language that we will be using to build our project. As per the top sites on the internet, the most popular languages for building web assembly projects are Rust, C, C++, and AssemblyScript. Other languages like Python, GoLang and .NET also provide support for web assemblies. All of the mentioned languages have a _compiler_ for compiling and running the program on webassembly. Before diving into details, let's analyze some major projects which have been developed using WebAsm.

### 1. Figma

Figma is a famous tool used to nowadays mostky for UI/UX design. It is a lighweight software which can also run on browsers. Figma uses **Emuscripten** to compile C/C++ code into WebAssembly which can run natively on the client's browser and allow users to do graphic intensive work without having the need to downlaod a desktop app.

### 2. Lichess

Lichess is an online chess-playing platform. It's engine is based on C++. It takes advantage of WebAssembly to perform complex calculations in the browser.

### 3. AutoCad Web

AutoCAD is a design tool for creating 2D and 3D drawings. It has been used as a desktop app form a long time. Now AutoCad has introduced a **Webapp** that allows you to uses AutoCad in the browser. It also uses C/C++ and the emuscripten compiler to compile it to web assembly.

### An Observation

As of now, major projects are using C++ for WebAsm projects.

## How will it work?

### If C++ is used:

- If we choose to use C++, we will need the emuscripten compiler to convert it into webassmebly.
- Then we need to 'glue' it to web environement using JavaScript.

### If Rust is Used:

For Rust, we can have two options,

- Build an entire application — an entire web app based in Rust.
- Build a part of an application — using Rust in an existing JavaScript frontend.

There is more support available for the latter, than building an entire Rust based application on WebAsm.

## C++ vs Rust: What should we prefer

| **Rust**                                      | **C++**                                         |
| --------------------------------------------- | ----------------------------------------------- |
| **Performance**                               |
| As Powerful as C++                            | Already a benchmark for performance             |
| **Memory Management**                         |                                                 |
| Better Memory Management                      | Bad MM as compared to RUST                      |
| **Support**                                   |                                                 |
| More support available                        | Support is available but no as much as for RUST |
| **Libraries and Modules**                     |                                                 |
| Lesser nuumber of modules(crates) available   | More libraries available                        |
| **Familiarity**                               |                                                 |
| Need to learn the language as it is new       | C++ has an advantage of being more familiar     |
| **Existing Projects**                         |                                                 |
| Quite a number of existing projects available | Most famous webasm projects are based on C++    |

### References

- https://developer.mozilla.org/en-US/docs/WebAssembly
- https://webassembly.org/docs
- https://www.figma.com/blog/webassembly-cut-figmas-load-time-by-3x/#:~:text=Because%20our%20product%20is%20written,that%20supports%20very%20large%20documents.
- https://www.codemotion.com/magazine/frontend/web-developer/getting-started-with-webassembly-and-rust/#:~:text=Rust%20code%20is%20just%20as,it%20into%20existing%20JavaScript%20projects.
- https://www.smashingmagazine.com/2019/04/webassembly-speed-web-app/
- https://madewithwebassembly.com/showcase/autocad/#:~:text=The%20AutoCAD%20web%20app%20uses,desktop%20applications%20on%20the%20web!
