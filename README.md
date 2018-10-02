# Herwig7-Local

<par>
To install localy use the instructions in http://herwig.hepforge.org/tutorials/installation/bootstrap.html  
<par/>
  
 <par> using the bootstrap script you can set all the required paths by sourcing the activate script supplied<par/>

```bash
source <HERWIGPATH>/bin/activate
```
 <par> as described in the message produced at the end of the bootstrap process. These variables can then be unset using <par/> 

```bash
deactivate
```
<par> 
As an example we study the Drell-Yan process at next-to-leading order (NLO). Copy the file LHC-Matchbox.in into your working directory.
<par/>
 
 ```bash
 cp <HERWIGPATH>/share/Herwig/LHC-Matchbox.in .
```
<par> Let’s read it<par/> 

```bash
Herwig read LHC-Matchbox.in
```

<par> 
 If you check the output you find the newly created run-file LHC-Matchbox.run in your working directory that contains all details of the event generator you have just set up. The subdirectory Herwig-scratch contains further output of the setup process.

We can now generate events with:
<par/> 
```bash
Herwig run LHC-Matchbox.run -N 100
  ```
