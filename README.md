# Forensic Artifact Collection Tool Matrix

Evaluation and comparison of different forensic artifact collection tools, also known as
forensic live collection.

What the emojis mean
* :sunny: Fully fulfilled requirement
* :partly_sunny: Partially fulfilled requirement
* :cloud: Tool doesn't fulfill feature or requirement

How the different requirements are weighted is left to the reader.

<!-- vim-markdown-toc GFM -->

* [Windows live collection tools](#windows-live-collection-tools)
* [Linux live collection tools](#linux-live-collection-tools)
* [MacOS live collection tools](#macos-live-collection-tools)
* [Contribution](#contribution)
* [License](#license)

<!-- vim-markdown-toc -->

##  Windows live collection tools

Initial tweet: https://twitter.com/swisscom_csirt/status/1301877750538567680

  | Requirement <br /> -------------- <br />Tool | independence of admin rights | flexible collection of artifacts and system configuration | external tool execution | free and open source | free download                                        | easy extensible                                                                        | multi-platform | one-shot binary                                         | output parsing                                                                                                        | active development                                                   | easy to use output format                               | 
  | :-------------                               | :-----:                      | :-----:                                                   | :-----:                 | :-----:              | :-----:                                              | :-----:                                                                                | :-----:        | :-----:                                                 | :-----:                                                                                                               | :-----:                                                              | :-----:                                                 | 
  | [KAPE](https://www.kroll.com/en/services/cyber-risk/investigate-and-respond/kroll-artifact-parser-extractor-kape)                                         | :cloud:                      | :sunny:                                                   | :sunny:                 | :cloud:              | :sunny: <br /> via online form, enterprise license                       | :sunny: <br /> [artifacts are open source](https://github.com/EricZimmerman/KapeFiles) and separated from the binary | :cloud:        | :cloud: <br /> .NET binary + config files for artifacts | :sunny:                                                                                                               | :sunny:                                                              | :sunny:                                                 | 
  | [Redline](https://www.fireeye.com/services/freeware/redline.html)                                      | :cloud:                      | :partly_sunny: <br /> limited set of predefined artifacts | :cloud:                 | :cloud:              | :sunny: <br /> via online form                       | :cloud:                                                                                | :cloud:        | :cloud:                                                 | :sunny:                                                                                                               | :partly_sunny: <br /> last change from June 8, 2018                  | :cloud: <br /> dedicated tool | 
  | [IRTriage](https://github.com/AJMartel/IRTriage)                                     | :cloud:                      | :sunny:                                                   | :sunny:                 | :sunny:              | :sunny:                                              | :cloud: <br /> AutoIt script and re-compilation                                        | :cloud:        | :cloud: <br /> third-party tools                        | :partly_sunny: <br /> RegRipper                                                        | :scream: <br />last change 4 years old                               | :sunny:                                                 | 
  | [IREC](https://binalyze.com/)                                         | :cloud:                      | :sunny:                                                   | :cloud:                 | :cloud:              | :sunny: <br /> via online form or commercial version | :cloud:                                                                                | :cloud:        | :sunny:                                                 | :partly_sunny: <br /> filesystem artifacts | :sunny:                                                              | :sunny:                                                 | 
  | [Invoke-LiveResponse](https://github.com/mgreen27/Invoke-LiveResponse)                          | :sunny:                      | :sunny:                                                   | :sunny:                 | :sunny:              | :sunny:                                              | :partly_sunny: <br /> PowerShell source code                                           | :cloud:        | :cloud: <br /> PowerShell scripts in subfolders         | :cloud:                                                                                                               | :partly_sunny:                                                       | :sunny:                                                 | 
  | [DFIR ORC](https://dfir-orc.github.io/)                                     | :cloud:                      | :sunny:                                                   | :sunny:                 | :sunny:              | :sunny:                                              | :cloud: <br /> C++ and re-compilation                                                  | :cloud:        | :sunny:                                                 | :partly_sunny:                                                                                                        | :sunny:                                                              | :sunny:                                                 | 
  | [CyLR](https://github.com/orlikoski/CyLR)                                         | :cloud:                      | :sunny:                                                   | :cloud:                 | :sunny:              | :sunny:                                              | :partly_sunny: <br /> .NET code and re-compilation                                     | :sunny:        | :sunny:                                                 | :cloud:                                                                                                               | :sunny:                                                              | :sunny:                                                 | 
  | [FastIR Collector](https://github.com/SekoiaLab/Fastir_Collector)                             | :cloud:                      | :sunny:                                                   | :partly_sunny:          | :sunny:              | :sunny:                                              | :partly_sunny: <br /> Python code and re-compilation                                   | :cloud:        | :sunny:                                                 | :cloud:                                                                                                               | :scream: <br />last change 3 years old                               | :sunny:                                                 | 
  | [artifactcollector](https://github.com/forensicanalysis/artifactcollector)                            | :cloud:                      | :sunny:                                                   | :sunny:                 | :sunny:              | :sunny:                                              | :partly_sunny: <br /> written in Go, prepare artifacts in YAML ([ForensicArtifacts](https://github.com/forensicartifacts/artifacts))         | :sunny:        | :sunny:                                                 | :cloud:                                                                                                               | :hatching_chick: <br /> young project on Github, only some month old | :partly_sunny:<br />artifactstore                       | 

Further reference: https://github.com/meirwah/awesome-incident-response#windows-evidence-collection

Other tools for artifact collection
* offline collection
  * [CrowdResponse](https://www.crowdstrike.com/resources/community-tools/crowdresponse/)
  * [Kansa](https://github.com/davehull/Kansa)
  * [Hoarder](https://github.com/muteb/Hoarder)
  * [Velociraptor](https://github.com/Velocidex/velociraptor)
  * [OSForensics](https://www.osforensics.com/osforensics.html)
  * [AChoir](https://github.com/OMENScan/AChoir)
* online collection
  * [F-Response](https://www.f-response.com)
  * [GRR](https://github.com/google/grr)
  * [Velociraptor](https://github.com/Velocidex/velociraptor)

## Linux live collection tools

Initial Tweet: https://twitter.com/swisscom_csirt/status/1341388348389244934

  | Requirement <br /> -------------- <br />Tool | independence of admin rights | flexible collection of artifacts and system configuration | external tool execution | free and open source | free download                                        | easy extensible                                                                        | multi-platform | one-shot binary                                         | output parsing                                                                                                        | active development                                                   | easy to use output format                               | 
  | :-------------                               | :-----:                      | :-----:                                                   | :-----:                 | :-----:              | :-----:                                              | :-----:                                                                                | :-----:        | :-----:                                                 | :-----:                                                                                                               | :-----:                                                              | :-----:                                                 | 
  | [Fast IR Artefacts](https://github.com/SekoiaLab/fastir_artifacts)                                         | :cloud:                      | :sunny: <br />[Forensics Artifact Repository](https://github.com/ForensicArtifacts/artifacts)                                                  | :sunny:                 | :sunny:              | :sunny:                        | :sunny: | :sunny:        | :cloud: <br />Require Python, pip and more  | :cloud:                                                                                                               | :sunny:                                                              | :sunny:                                                 | 
  | [Live Response Collection](https://www.brimorlabs.com/tools/)                                      | :cloud:                      | :cloud:  | :sunny:                 | :sunny:              | :sunny:                       | :sunny:                                                                                | :sunny:        | :cloud:                                                 | :cloud:                                                                                                               | :sunny:                   | :sunny:  | 
  | [ir-rescue](https://github.com/diogo-fernan/ir-rescue)                                     | :cloud:                      | :cloud:                                                  | :sunny:                 | :sunny: <br /> Commercial usage needs permission             | :sunny:                                              | :sunny: <br /> (Bash v4+)                                        | :sunny:        | :cloud: <br /> [AVML](https://github.com/microsoft/avml) for memory dump                       | :cloud:                                                         | :sunny:                               | :sunny:                                                 | 
  | [CyLR](https://github.com/orlikoski/CyLR)                                         | :sunny:                      | :sunny:                                                   | :cloud:                 | :sunny:              | :sunny:  | :partly_sunny: <br /> .NET code and recompilation                                                                               | :sunny:        | :sunny: <br />.NET Binary                                                 | :cloud:  | :partly_sunny: <br />[Open Letter to the users](https://docs.google.com/document/d/1L6CBvFd7d1Qf4IxSJSdkKMTdbBuWzSzUM3u_h5ZCegY/edit?usp=sharing)                                                             | :sunny:                                                 | 
  | [artifactcollector](https://github.com/forensicanalysis/artifactcollector)                          | :cloud:                      | :sunny: <br />[Forensics Artifact Repository](https://github.com/ForensicArtifacts/artifacts)                                                   | :sunny:                 | :sunny:              | :sunny:                                              | :partly_sunny: <br /> Prepare artifacts in YAML and Go compilation                                           | :sunny:        | :sunny:          | :cloud:                                                                                                               | :sunny:                                                       | :partly_sunny: <br />ArtefactStore                                                | 
  
Further reference: https://github.com/meirwah/awesome-incident-response#linux-evidence-collection

Other tools for artifact collection
* online collection
  * [F- Response TACTICAL](https://www.f-response.com/software/tac)

## MacOS live collection tools

Tools for artifact collection
  * [mac_apt - macOS (and iOS) Artifact Parsing Tool](https://github.com/ydkhatri/mac_apt) - mac_apt is a DFIR (Digital Forensics and Incident Response) tool to process Mac computer full disk images (or live machines) and extract data/metadata useful for forensic investigation. It is a python based framework, which has plugins to process individual artifacts (such as Safari internet history, Network interfaces, Recently accessed files & volumes, ..).
  * [macOS Artifact Collector (macosac)](https://github.com/mnrkbys/macosac) - This is a DFIR tool for collecting artifact files on macOS. The "Extended Attributes" of artifact files are collected too. Furthermore, this tool can collect artifacts in Time Machine backups as well as ones on the current disk. This tool does not provide features for analyzing artifacts, so you can analyze them with your favorite artifact analyzing tools.
  * [AutoMacTC: Automated Mac Forensic Triage Collector](https://github.com/CrowdStrike/automactc) - This is a modular forensic triage collection framework designed to access various forensic artifacts on macOS, parse them, and present them in formats viable for analysis. The output may provide valuable insights for incident response in a macOS environment. Automactc can be run against a live system or dead disk (as a mounted volume.)
  * [OSXCollector](https://github.com/Yelp/osxcollector) - [ARCHIVED] OSXCollector is a forensic evidence collection & analysis toolkit for OSX.
  * [OSXAuditor](https://github.com/jipegit/OSXAuditor) - [NO LONGER MAINTAINED] OS X Auditor is a free Mac OS X computer forensics tool. OS X Auditor parses and hashes the various artifacts on the running system or a copy of a system you want to analyze. Forked by Yelp into osxcollector.

References
* [OSX Forensics: a brief selection of useful tools](https://www.andreafortuna.org/2020/12/07/osx-forensics-a-brief-selection-of-useful-tools/)
* [OS X forensic acquisition: a basic workflow](https://www.andreafortuna.org/2019/08/15/os-x-forensic-acquisition-a-basic-workflow/)
* [Mac4n6 Group](https://github.com/pstirparo/mac4n6) - Interested in Mac OS X and iOS Forensics? We are collecting and maintaining a list of mac4n6 resources.

## Contribution

Please fill an issue or make a pull request to improve the table, add tools
and correct how we rated the coverage for a requirement.

## License

[![License: CC BY-SA 4.0](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/)

The work by Swisscom CSIRT is licensed under a 
[Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)
License](https://creativecommons.org/licenses/by-sa/4.0/).

ArtifactCollectionMatrix is free to use. It is licensed under the Creative
Commons Attribution-ShareAlike 4.0 license, so you can copy,
distribute and transmit the work, and you can adapt it, and use it
commercially, but all provided that you attribute the work and if you alter,
transform, or build upon this work, you may distribute the resulting work only
under the same or similar license to this one.
