# build-recipes
Collection of build recipes for Visual Studio projects. Clone build-recipes as a submodule into your project and add the property sheets to your MSBuild projects. We assume the following project structure:

```
  Root of [devkit]
    |-> build-recipes [submodule]
    |-> [devkit project 1 submodule]
      |-> build
        |-> [devkit project 1 project]
          |-> [devkit project 1 project.vsxproj] // references build-recipes property sheets
    |-> [devkit project 2 submodule]
      |-> build
        |-> [devkit project 2 project]
          |-> [devkit project 2 project.vsxproj] // references build-recipes property sheets
    |-> ... continue using the same scheme for other projects
    |-> [devkit solution folder 1]
      |-> [devkit solution.sln] // references projects.vsxproj
```
