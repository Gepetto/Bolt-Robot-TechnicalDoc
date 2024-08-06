# Bolt robot technical document

## Description

This a latex project explaining the technical details of the Bolt robot.

The first document entitled "Technical Documentation for Bolt Estimator" explains the concepts behind the state estimator used on the robot.

## Build the pdf

For a simple build please run:
```bash
make
```

## Editing the project.

With a little bit of dependency you can simulate the behavior of overleaf locally.
The dependency are:
- okular (`sudo apt install okular`)
- vscode (`snap install vscode`)
- inotify-wait (`sudo apt install inotify-tools`)
- latex_edition_scripts (it comes as a git submodule here).

In order to activate the git submodule you can:
- directly clone the project with the submodule activated:
```bash
git clone --recursive git@github.com:nnniels/Bolt-Robot-TechnicalDoc.git
```
- Activate the submodule after the clone:
```bash
cd Bolt-Robot-TechnicalDoc
git submodule update --init
```

Then simply:
```bash
cd Bolt-Robot-TechnicalDoc
./latex_edition_script/edition.launch
```
This will:
- open okular for output visualization
- open vscode for the latex editing
- rebuild every time you save a file in the latex project.
