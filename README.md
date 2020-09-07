# Forensic Artifact Collection Tool Matrix

Evaluation of different artifact collection tools.

What the emojis mean
* :sunny: Fully fulfilled requirement
* :partly_sunny: Partially requirement
* :cloud: Tool doesn't cover feature or requirement

##  Windows live collection tools

Initial tweet: https://twitter.com/swisscom_csirt/status/1301877750538567680

| Requirement <br /> -------------- <br />Tool | independence of admin rights | flexible collection of artifacts and system configuration  | external tool execution | free and open source | free download | easy extensible | multi-platform | one-shot binary | output parsing | active development | easy to use output format |
| :------------- | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: |
| KAPE |:cloud:|:sunny: |||:sunny:|:sunny:|:cloud:||||:sunny:|
| Redline |:cloud:| :partly_sunny: <br /> limited set of predefined artifacts |||:sunny:||:cloud:|||| :cloud: <br /> dedicated tool used to analyse artifacts|
| IRTriage |:cloud:| :sunny: |||:sunny:||:cloud:|||:scream: <br />last change 4 years old |:sunny:|
| IREC | :cloud: | :sunny: | ||:sunny:||:cloud:||||:sunny:|
| Invoke-LiveResponse | :sunny: |  :sunny:|:sunny: |:sunny:|:sunny:||:cloud:||||:sunny:|
| DFIR ORC | :cloud: |:sunny:  |:sunny: |:sunny:|:sunny:||:cloud:||||:sunny:|
| CyLR | :cloud: |:sunny:  | ||:sunny:||:sunny:||||:sunny:|
| FastIR Collector | :cloud: | :sunny: | |:sunny:|:sunny:||:cloud:|||:scream: <br />last change 3 years old |:sunny:|
| artifactcollector | :cloud: |:sunny:  |:sunny: |:sunny:|:sunny:|:partly_sunny:|:sunny:||| :hatching_chick: <br /> young project on Github, only some month old |:partly_sunny:<br />artifactstore|


Further reference: https://github.com/meirwah/awesome-incident-response#windows-evidence-collection 

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
