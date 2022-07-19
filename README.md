# UCSF_work
work in progress
trying changes

To run the pipeline in c4-ucsf cluster

0. Don't forget to get into tmux for efficiency

1. Log in into c4-dev1 node
2. Load the virtual env (https://www.c4.ucsf.edu/howto/python.html)
	[sermare@c4-dev1:~]$ cd python/ATAC_project/
	[sermare@c4-dev1:~]$ . bin/activate
4. Load java 
	(ATAC_proj) [sermare@c4-dev1:~]$ export JAVA_HOME=/c4/home/sermare/jdk-11.0.2
	(ATAC_proj) [sermare@c4-dev1:~]$ export PATH=$PATH:$JAVA_HOME/bin
5. Verify java 
	(ATAC_proj) [sermare@c4-dev1:~]$ java --version
		openjdk 11.0.15 2022-04-19 LTS
		OpenJDK Runtime Environment 18.9 (build 11.0.15+9-LTS)
		OpenJDK 64-Bit Server VM 18.9 (build 11.0.15+9-LTS, mixed mode, sharing)
6. Verify caper is working 
	(ATAC_proj) [sermare@c4-dev1:~]$ caper init
7. Edit the template.json file

8. caper run ../atac-encode-pipeline/atac.wdl -i template.json --singularity
