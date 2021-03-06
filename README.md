An experiment on using CNNs to predict pressure fields around airfoils, based on ground truth pressure fields generated by a CFD solver. For more details, see the [blog post](http://sam.pfrommer.us/fast-estimation-of-airfoil-pressure-fields-using-deep-convolutional-neural-networks) and [full report](https://github.com/spfrommer/airfoil-pressure-learning/blob/master/report.pdf).

## FOR TRAINING
### Requirements
Just go into airsim/train and pip install requirements.txt

### Running
python airsim/train/train.py
To visualize output, run:
tensorboard --logdir=./out/training/runs

## FOR GENERATING DATA
### Requirements
Python 2.7
pip
OpenFoam 5.x
gmsh 2.10.1

### Installing on Linux
sudo apt install python2.7 python-pip

sudo sh -c "wget -O - http://dl.openfoam.org/gpg.key | apt-key add -"
sudo add-apt-repository http://dl.openfoam.org/ubuntu
sudo apt-get update
sudo apt-get -y install openfoam5

sudo apt-get install gmsh

pip install -r requirements.txt
npm install

### Running
python airsim/generate/generate.py
