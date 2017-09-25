# CSCD439 - Fall 2017
## Installing Software for Machine Learning

1. Install Virtual Box ( **If you are running ubuntu 16.04 on your system, then you can skip to step 3 below.**)

	go to [VirtualBox Wiki Downloads](https://www.virtualbox.org/wiki/Downloads) and download the version of VB appropriate for your base operating system.  

	Installation details can be found [here](https://www.virtualbox.org/manual/ch02.html).

2. Install Ubuntu 16.04.  go to [this page](https://www.ubuntu.com/download) and download the ubuntu 16.04 desktop image.

3. Log in and update and upgrade the system.

	```
	sudo apt-get update
	sudo apt-get upgrade
	```
	
4. Install [Guest Additions](https://www.virtualbox.org/manual/ch04.html) in the ubuntu client.
	
5. Install prereqs for virtual environment:

	```
	sudo apt-get install build-essential python3-dev python3-setuptools python3-tk
	```

6. Install [python virtual environment](https://gist.github.com/FarhadurFahim/73c0fad6350332cef7a653bcd762f08d)

7. Create and activate a virtual environment for testing.

	```
	virtualenv testve
	source testve/bin/activate
	```
	
8. Now, in the virtual environment, install pandas, statsmodel, and scikit-learn.

	```
	pip install -U numpy scipy
	pip install -U pandas statsmodels
	pip install -U scikit-learn
	pip install -U matplotlib
	```
	
9. install ipython and jupyter.

	```
	pip install -U ipython jupyter
	```

10. Test using jupyter notebook.  

	First go to the testve folder and create a notebook folder. then run jupyter

	```
	cd testve
	mkdir project_notebook
	jupyter notebook
	```
	Your browser will open up.  in the browser, you will see this:
	![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")