# This is a environment Setup Tool

An **environment** refers to the setup in which code runs—this includes the programming language version, libraries, dependencies, and configurations. Virtual environments are especially important in languages like Python because they allow developers to isolate projects from each other. Without them, different projects on the same system might require conflicting versions of libraries or packages, leading to errors and instability. By creating a virtual environment, each project gets its own dedicated space with the exact dependencies it needs, ensuring consistency, reproducibility, and easier collaboration across machines and teams.


# Languages And their Environments

1.  **Python** – Popular for web, AI, and data science. Virtual environments manage dependencies cleanly. Prevents conflicts between projects.
    
2.  **Java** – Used in enterprise apps and Android. Requires JDK setup for compiling and running. Classpath and versioning matter for stability.
    
3.  **C** – Systems programming and embedded. Needs a compiler like GCC/Clang. Environment ensures proper linking and libraries.
    
4.  **C++** – High-performance apps and games. Setup requires compilers and build tools. Environment ensures correct standard libraries and dependencies.
    
5.  **JavaScript (Node.js)** – Web and backend scripting. Needs Node and npm for package management. Project environments handle versioned dependencies.
    
6.  **TypeScript** – Superset of JavaScript with types. Requires TypeScript compiler and Node. Environment setup ensures compatibility and builds.
    
7.  **C# (.NET)** – Enterprise, desktop, and game dev. Uses .NET SDK and runtime. Environments define framework version and libraries.
    
8.  **Go** – Modern systems/backend language. Uses `go mod` for modules. Environment ensures reproducibility and fast builds.
    
9.  **Rust** – Memory-safe, fast systems language. Managed by Cargo (package manager). Environment handles dependencies and compilation.
    
10.  **Ruby** – Web and scripting (Rails). Uses Bundler for dependencies. Environments ensure gem compatibility.
    
11.  **PHP** – Web backend scripting. Requires PHP runtime and Composer. Environments help with framework/library versions.
    
12.  **Swift** – iOS/macOS apps. Uses Swift Package Manager. Environments ensure compatibility with Apple SDKs.
    
13.  **Kotlin** – Android and backend apps. Requires JVM or Android SDK. Environment ensures smooth Java interop.
    
14.  **Scala** – Functional + OOP on JVM. Uses sbt for builds. Environment setup keeps library versions aligned.
    
15.  **R** – Statistical computing and data science. Uses CRAN packages. Environments ensure reproducible research.
    
16.  **Perl** – Text processing and scripting. Uses CPAN for modules. Environment keeps modules project-specific.
    
17.  **Dart (Flutter)** – Web and mobile apps. Needs Dart SDK or Flutter. Environments ensure consistent build and deployment.
    
18.  **Julia** – Scientific computing and ML. Uses environments via `Pkg`. Ensures reproducible numerical experiments.
    
19.  **MATLAB/Octave** – Numerical computing. Uses package/toolbox installations. Environment setups manage dependencies for simulations.
    
20.  **Shell (Bash)** – Automation and scripting. Needs correct runtime/shell. Environments manage execution context and dependencies.



## Python Environment Creation

# Python Virtual Environment Setup

A **virtual environment** in Python is a self-contained directory that contains its own Python installation and packages.  
It allows you to isolate project dependencies, avoid version conflicts, and ensure reproducibility across different systems.

---

###  Why Use a Virtual Environment?

- Prevents dependency conflicts between projects.  
- Keeps your global Python installation clean.  
- Makes projects reproducible on different machines.  
- Commonly used in web development, data science, and ML workflows.

---


### Prerequisites

- Install **Python 3.6 or later** on your system.  
- Verify the installation by running one of the following commands in your terminal:

  ```bash
  python --version

## Creating a Virtual Environment

###  Windows
<p> Activate windows in the project folder using following commands.</p>

```bash
cd project_folder
```

```bash
python -m venv env 
or 
python3 -m venv env 
```
### Activating Virtual Environment 
<p> Using the command to activate the virutal environment in the project_folder.  </p>

#### Command Prompt
```bash 
env\Scripts\activate
```

#### Power Shell 
```bash 
.\env\Scripts\Activate.ps1
```

#### macOS / Linux
```bash 
source env/bin/activate
```

#### Deactivating the environment 
```bash 
deactivate
```



### Installing Packages
Inside the environment, use **pip**:

`pip install package_name` 

Freeze dependencies for reproducibility:

`pip freeze > requirements.txt` 

Reinstall them later with:

`pip install -r requirements.txt`


### Removing the environment 
Simply delete the folder:

`rm -rf env` 

On **Windows**:

`rmdir /s /q env`
