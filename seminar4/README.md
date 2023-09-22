# seminar-4

## Prerequisites

### Step 1.

Pull docker image from docker registry:  
``` docker pull miykael/nipype_tutorial:latest ```  
(make sure that docker daemon on your computer is working)  
In case of any troubles please read this [instruction](docker pull miykael/nipype_tutorial:latest)
### Step 2.
Clone this repository.

### Step 3.
Download dataset [tar (for unix users)](https://disk.yandex.ru/d/ZtGS5A4VXt1Eyw). Move the archive to the seminar 4 directory.  And unarchive it (if you are using unix like system just run ```tar -xf <ARCHIVE_NAME>.tar```, if you are a windows user, please follow this [instruction](https://wiki.haskell.org/How_to_unpack_a_tar_file_in_Windows))

### Step 4.
Run this command to run docker container with mounted directory of the seminar.  

```docker run -it --rm -p 8888:8888 -v <PATH_TO_SEMINAR_4_ON_YOUR_PC>:/home/neuro/nipype_tutorial/notebooks/seminar miykael/nipype_tutorial jupyter notebook ```  
Note that ```<PATH_TO_SEMINAR_4_ON_YOUR_PC>``` is a global path to the seminar 4 directory on your computer.  
Don't forget to copy the token of your jupyter server (check the terminal). Then detach your container (```CTRL+P+Q```) just in case. If everything is okay, the jupyter server can be reached at http://localhost:8888/.  

#### Dataset:
* A test-retest fMRI dataset for motor, language and spatial attention functions https://www.openfmri.org/dataset/ds000114/
