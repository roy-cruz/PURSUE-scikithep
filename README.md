# PURSUE Scikit-HEP Workshop
This repository holds all of the material & links which will be used in the PURSUE Scikit-HEP tutorial. To guide the learning process, we will be utilizing the following material kindly provided by HSF:
* [HSF Uproot Tutorial](https://masonproffitt.github.io/uproot-tutorial/) 
* [HSF Scikit-HEP Tutorial](https://hsf-training.github.io/hsf-training-scikit-hep-webpage/).

# Setup

## LPC 

We can set up a CMSSW environment with all of the neccesary tools we need. For this, connect to the LPC Cluster using the following command

```bash
ssh -Y <user>@cmsplc-el8.fnal.gov -L 8888:localhost:8888
```

After connecting, run the following set of commands
```bash
mkdir -p ~/nobackup/pursue-scikithep/
cd ~/nobackup/pursue-scikithep/
git clone git@github.com:roy-cruz/PURSUE-scikithep.git
cmsrel CMSSW_12_4_20
cd CMSSW_12_4_20; cmsenv; cd -
cd PURSUE-scikithep
jupyter notebook --no-browser --port=8888
```

Paste the link that appears in your browser and you are ready to go!

## Virtual Environment

In your working directory, clone this repository by running the following command.

```bash
git clone git@github.com:roy-cruz/PURSUE-scikithep.git
```

Next, create the required virtual environment by running the following commands

```bash
python3 -m virtualenv venv
source ./venv/bin/activate
pip3 install poetry
cd PURSUE-scikithep
poetry install --no-root
```

Once everything finishes installing, go ahead and start up a Jupyter session by running

```bash
jupyter notebook --no-browser
```

and copy the given link into your browser.



<!-- * Hitting the `.` button.
* Clicking [here](https://github.dev/roy-cruz/PURSUE-scikithep).

Once the page loads, click on the blue "GitHub" button on the bottom left, and select "Continue Working in GitHub Codespaces" in the drop down menu that appears. Once your Codespace finishes loading, open the terminal (upper right corner), and run the following commands to create a virtual environment with all of the required packages

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

All set! Now you can run the included notebooks in addition to any notebook you wish to create to work in.

## Google Colab -->
