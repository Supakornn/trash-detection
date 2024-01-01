Trash_ICRA19 Dataset 

Michael Fulton, Jungseok Hong, Junaed Sattar
Related Paper: https://ieeexplore.ieee.org/abstract/document/8793975

IF USING CITE THE ABOVE PAPER.


For questions, issues, etc, contact: irvlab@umn.edu
----------------------------------------------------------------
This folder contains YOLO configurations and weights. 

The repository and commit used for generating the results shown in the related paper is:
https://github.com/AlexeyAB/darknet/tree/cad4d1618fee74471d335314cb77070fee951a42

Software Heritage's archive of the repository: https://archive.softwareheritage.org/swh:1:rev:cad4d1618fee74471d335314cb77070fee951a42;origin=https://github.com/AlexeyAB/darknet;visit=swh:1:snp:ae6a6472c0c65ac0c1ca42e08766c79f53a761d3/

No guarentees are made about these cfg and weights working for later commits.


There are four versions of the files here, for four different networks/trainings based on YOLO. 
They are:
	- yolo (yolo, fine tuned on the Trash-ICRA19 dataset)
	- tiny_yolo (tiny yolo, fine tuned on the Trash-ICRA19 dataset)
	- yolo_tl_last2 (yolo, trained via transfer learning on the last two layers only)
	- yolo_tl_last3 (yolo, trained via transfer learning on the last three layers only)
	
	
For each version, there is a:
	- .weights file in the weights/ folder (This is the weights of the network used in the paper)
	- .cfg file in the cfg/ folder (This is the network definition used by darknet)
	- .data file in the cfg/ folder (This is the config file with paths to the files needed by darknet to train)
	

Also in the cfg folder are the following files:
	- yolo.names (List of the names of the classes for display)
	- train.txt (Paths to all files in the train set)
	- test.txt (Paths to all files in the test set)
	- val.txt (Paths to all files in the val set)	
