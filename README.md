# Forensic Artifact Collection Tool Matrix

Evaluation of different artifact collection tools for Windows, also known as
live collection.

What the emojis mean
* :sunny: Fully fulfilled requirement
* :partly_sunny: Partially requirement
* :cloud: Tool doesn't cover feature or requirement

How the different requirements are weighted is left to the reader.

<!-- vim-markdown-toc GFM -->

* [Windows live collection tools](#windows-live-collection-tools)
* [Contribution](#contribution)
* [License](#license)

<!-- vim-markdown-toc -->

##  Windows live collection tools

Initial tweet: https://twitter.com/swisscom_csirt/status/1301877750538567680

  | Requirement <br /> -------------- <br />Tool | independence of admin rights | flexible collection of artifacts and system configuration | external tool execution | free and open source | free download                                        | easy extensible                                                                        | multi-platform | one-shot binary                                         | output parsing                                                                                                        | active development                                                   | easy to use output format                               | 
  | :-------------                               | :-----:                      | :-----:                                                   | :-----:                 | :-----:              | :-----:                                              | :-----:                                                                                | :-----:        | :-----:                                                 | :-----:                                                                                                               | :-----:                                                              | :-----:                                                 | 
  | KAPE                                         | :cloud:                      | :sunny:                                                   | :sunny:                 | :cloud:              | :sunny: <br /> via online form                       | :sunny: <br /> artifacts are open source and separated from the binary | :cloud:        | :cloud: <br /> .NET binary + config files for artifacts | :sunny:                                                                                                               | :sunny:                                                              | :sunny:                                                 | 
  | Redline                                      | :cloud:                      | :partly_sunny: <br /> limited set of predefined artifacts | :cloud:                 | :cloud:              | :sunny: <br /> via online form                       | :cloud:                                                                                | :cloud:        | :cloud:                                                 | :sunny:                                                                                                               | :partly_sunny: <br /> last change from June 8, 2018                  | :cloud: <br /> dedicated tool | 
  | IRTriage                                     | :cloud:                      | :sunny:                                                   | :sunny:                 | :sunny:              | :sunny:                                              | :cloud: <br /> AutoIt script and re-compilation                                        | :cloud:        | :cloud: <br /> third-party tools                        | :partly_sunny: <br /> RegRipper                                                        | :scream: <br />last change 4 years old                               | :sunny:                                                 | 
  | IREC                                         | :cloud:                      | :sunny:                                                   | :cloud:                 | :cloud:              | :sunny: <br /> via online form or commercial version | :cloud:                                                                                | :cloud:        | :sunny:                                                 | :partly_sunny: <br /> filesystem artifacts | :sunny:                                                              | :sunny:                                                 | 
  | Invoke-LiveResponse                          | :sunny:                      | :sunny:                                                   | :sunny:                 | :sunny:              | :sunny:                                              | :partly_sunny: <br /> PowerShell source code                                           | :cloud:        | :cloud: <br /> PowerShell scripts in subfolders         | :cloud:                                                                                                               | :partly_sunny:                                                       | :sunny:                                                 | 
  | DFIR ORC                                     | :cloud:                      | :sunny:                                                   | :sunny:                 | :sunny:              | :sunny:                                              | :cloud: <br /> C++ and re-compilation                                                  | :cloud:        | :sunny:                                                 | :partly_sunny:                                                                                                        | :sunny:                                                              | :sunny:                                                 | 
  | CyLR                                         | :cloud:                      | :sunny:                                                   | :cloud:                 | :sunny:              | :sunny:                                              | :partly_sunny: <br /> .NET code and re-compilation                                     | :sunny:        | :sunny:                                                 | :cloud:                                                                                                               | :sunny:                                                              | :sunny:                                                 | 
  | FastIR Collector                             | :cloud:                      | :sunny:                                                   | :partly_sunny:          | :sunny:              | :sunny:                                              | :partly_sunny: <br /> Python code and re-compilation                                   | :cloud:        | :sunny:                                                 | :cloud:                                                                                                               | :scream: <br />last change 3 years old                               | :sunny:                                                 | 
  | artifactcollector                            | :cloud:                      | :sunny:                                                   | :sunny:                 | :sunny:              | :sunny:                                              | :partly_sunny: <br /> Go, prepare artifacts in YAML and Go re-compilation              | :sunny:        | :sunny:                                                 | :cloud:                                                                                                               | :hatching_chick: <br /> young project on Github, only some month old | :partly_sunny:<br />artifactstore                       | 


Further reference: https://github.com/meirwah/awesome-incident-response#windows-evidence-collection 

## Contribution

Please fill an issue or make a pull request to improve the table, add tools
and correct how we rated the coverage for a requirement.

## License

[![License: CC BY-SA 4.0](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/)

The content of this project is licensed under a 
[Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)
License](https://creativecommons.org/licenses/by-sa/4.0/).

ArtifactCollectionMatrix is free to use. It is licensed under the Creative
Commons Attribution-ShareAlike 4.0 license, so you can copy,
distribute and transmit the work, and you can adapt it, and use it
commercially, but all provided that you attribute the work and if you alter,
transform, or build upon this work, you may distribute the resulting work only
under the same or similar license to this one.
