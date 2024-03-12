# PURSUE Scikit-HEP Workshop
This repository holds all of the material which will be used in the PURSUE Scikit-HEP tutorial. The material presented will be (a version of) what can be found in the [HSF Uproot Tutorial](https://masonproffitt.github.io/uproot-tutorial/) and the [HSF Scikit-HEP Tutorial](https://hsf-training.github.io/hsf-training-scikit-hep-webpage/).

# Setup
## GitHub Codespace
From this repository, open a GitHub Codespace by either

* Hitting `.`
* Clicking [here](https://github.dev/roy-cruz/PURSUE-scikithep)

Once the page loads, click on the blue "GitHub" button on the bottom left, and select "Continue Working in GitHub Codespaces" in the drop down menu that appears. Once your Codespace finishes loading, open the terminal (upper right corner), and run the following commands to create a virtual environment with all of the required packages

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

All set! Now you can run the included notebooks in addition to any notebook you wish to create to work in.