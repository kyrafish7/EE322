# Lab 9 - YANG

## Installation
#### First step of this lab was to install the needed python packages it was installed using pip like the previous packages
![image](Images/Lab9install.png)

## Pyang
#### Then I copied intrusiondetection.yang into demo and moved to the demo directory
![image](Images/Lab9_1.png)
#### I then executed the following commands to create `intrusiondetection.yin` and `intrusiondetection.uml` version of it in .yang, .yin, and .uml forms
#### `cat intrusiondetection.yang`
#### `pyang -f yin -o intrusiondetection.yin intrusiondetection.yang`
#### `cat intrusiondetection.yin`
#### `pyang -f uml -o intrusiondetection.uml intrusiondetection.yang --uml-no=stereotypes,annotation,typedef`
#### `cat intrusiondetection.uml`
![image](Images/Lab9_2.png)
![image](Images/Lab9_3.png)

## PlantUML
#### I then ran the command `python3 -m plantuml intrusiondetection.uml` to create a diagram in PNG format. Then I installed and ran GIMP and Pinta in order to view the PNG file
![image](Images/Lab9install2.png)

## PNG Image Result
![image](Images/Lab9final.png)

