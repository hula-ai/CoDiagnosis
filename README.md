# CoDiagnosis
### Running the OHIF Viewer

1. Fork the repository of OHIF Viewer from Github: https://docs.github.com/en/get-started/quickstart/fork-a-repo#:~:text=Forking%20a%20repository%201%20On%20GitHub.com%2C%20navigate%20to,Copy%20the%20DEFAULT%20branch%20only.%20...%20More%20items

*the following commands are meant to be used in command prompt*
2. [Clone your forked repository][how-to-clone]
   - `git clone https://github.com/GITHUB-USERNAME/Viewers.git`
3. Navigate to the cloned project's directory using linux commands 
   -  `cd DIRECTORYNAME\`
4. Add the original online repo as a `remote` named `upstream`
   - `git remote add upstream https://github.com/OHIF/Viewers.git`
####Setting up the DICOM Server to put Custom Data in the OHIF Viewer:
1. Download docker for Windows
2. open command prompt and run `wsl --update`
2. run `docker --version` to make sure that Docker is installed
3. Download OrthanC

This video contains the televised instructions: https://youtu.be/BwRBvEMl_b8

## Running the program

-- The received images should show up in the UI of the Archive at http://localhost:8080/dcm4chee-arc/ui2 or https://localhost:8443/dcm4chee-arc/ui2:

run `git clone https://github.com/hyper4saken/ohif-orthanc.git`
run `cd ohif-orthanc`
run `docker-compose pull`
run `docker-compose up -d`
6. paste "localhost:8042" and "localhost:3000" into your browser to activiate the upload portal and the OHIF Viewer(old windows explorer will not work)
7. when asked to log in, enter the following credentials:
Username: mapdr
Password: changestrongpassword

#Closing the Program
To close the program, simply run `docker-compose stop` and the program will stop running.
