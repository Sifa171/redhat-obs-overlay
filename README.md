## Red Hat OBS overlay
-----------------

This repository contains all necessary files for your personal Red Hat OBS overlay.

![alt text](https://github.com/Sifa91/redhat-obs-overlay/blob/master/img/readme/example.PNG "Overlay example")

### Setup

#### Prerequesites

First of all you need [OBS](https://obsproject.com/) installed on your computer.
At second you need a plugin to create a virtual cam, which you can use later in your browser as your webcam.
[Virtual cam for Windows](https://obsproject.com/forum/resources/obs-virtualcam.539/)
Virtual cam for Linux and Mac? ---> Will be added later


#### Installing the overlay with ansible

Clone this repo!
```
git clone https://github.com/Sifa91/redhat-obs-overlay.git
```
Navigate to the cloned repository on your shell and adjust the variable in `ansible/vars.yml`. <br>
Care! Do not end with a '/'

```
overlay_path: "PATH_TO_YOUR_CLONED_REPOSITORY"
```

Execute: 
```
ansible-playbook ansible/install.yml
```

Then open your OBS and import overlay.json from the cloned repository.
In your OBS go to Scene collection -> Import 

DONE!!!


