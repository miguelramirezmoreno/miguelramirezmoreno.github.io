---
layout: archive
title: "Matlab Cheatsheet"
permalink: /matlab_cheatsheet/
author_profile: true
---
This is a cheatsheet of operations for image analysis using Matlab

## Directory operations

### Chose a main directory to analyze (prompts a choice by the user)

```
currentFolder = pwd;
addpath(pwd);
main_directory= uigetdir();
```
### Generate a variable with existing directory (script will stop if not found)
```
variable_name = [main_directory, 'directory_location_from_current_directory'];
```

### Create a directory within main one if it does not exist (directory won't be assigned a variable without calling it after

```
if exist([main_directory, '/directory_name'],'dir')==0
    mkdir(main,'/directory_name');
end
```

### find files inside directory

## Loading images

## generate image and save them

```
cd(directory);
imshow(image);
hold on;
image_name= 'image_name.extension'];
print(image, image);
close all

Check the documentation for all the possible inputs (specially important to check the supported formats): https://uk.mathworks.com/help/matlab/ref/print.html#bukyb6e-1-formatoptions
