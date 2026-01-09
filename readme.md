Machine Learning Notebooks, 3rd edition
This project aims at teaching you the fundamentals of Machine Learning in python. It contains the example code and solutions to the exercises in the third edition of my O'Reilly book Hands-on Machine Learning with Scikit-Learn, Keras and TensorFlow (3rd edition):

book

Note: If you are looking for the second edition notebooks, check out ageron/handson-ml2. For the first edition, see ageron/handson-ml.

Quick Start
Want to play with these notebooks online without having to install anything?
Open In Colab (recommended)
⚠ Colab provides a temporary environment: anything you do will be deleted after a while, so make sure you download any data you care about.

Details
Just want to quickly look at some notebooks, without executing any code?
Render nbviewer

github.com's notebook viewer also works but it's not ideal: it's slower, the math equations are not always displayed correctly, and large notebooks often fail to open.

Want to run this project using a Docker image?
Read the Docker instructions.

Want to install this project on your own machine?
Start by installing Anaconda (or Miniconda), git, and if you have a TensorFlow-compatible GPU, install the GPU driver, as well as the appropriate version of CUDA and cuDNN (see TensorFlow's documentation for more details).

Next, clone this project by opening a terminal and typing the following commands (do not type the first $ signs on each line, they just indicate that these are terminal commands):

$ git clone https://github.com/ageron/handson-ml3.git
$ cd handson-ml3
Next, run the following commands:

$ conda env create -f environment.yml
$ conda activate homl3
$ python -m ipykernel install --user --name=python3
Finally, start Jupyter:

$ jupyter notebook
If you need further instructions, read the detailed installation instructions.

FAQ
Which Python version should I use?

I recommend Python 3.10. If you follow the installation instructions above, that's the version you will get. Any version ≥3.7 should work as well.

I'm getting an error when I call load_housing_data()

If you're getting an HTTP error, make sure you're running the exact same code as in the notebook (copy/paste it if needed). If the problem persists, please check your network configuration. If it's an SSL error, see the next question.

I'm getting an SSL error on MacOSX

You probably need to install the SSL certificates (see this StackOverflow question). If you downloaded Python from the official website, then run /Applications/Python\ 3.10/Install\ Certificates.command in a terminal (change 3.10 to whatever version you installed). If you installed Python using MacPorts, run sudo port install curl-ca-bundle in a terminal.

I've installed this project locally. How do I update it to the latest version?

See INSTALL.md

How do I update my Python libraries to the latest versions, when using Anaconda?

See INSTALL.md