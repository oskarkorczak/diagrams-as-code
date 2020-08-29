# [Diagrams as code][dac]

Keep all architectural diagrams as code in repository. All diagrams can be generated from Python source files. 


## Prerequisites

The project requires:

 * [Python 3.6 or higher](https://diagrams.mingrammer.com/docs/getting-started/installation); check you Python version `python --version`
 * `graphviz` executable has to be on path; install with brew `brew install graphviz`
 
## Virtual environment
Create local environment an import all required dependencies:

```
python -m venv local
python --version
source local/bin/activate

pip install -r requirements.txt
```

When work in the repository is finished, bear in mind that virtual environment has to be deactivated:

```
deactivate
```


## Running 
Generate PNG image based on Python diagram definition

```
python diagram-definition.py
```

Diagram definition script will generate PNG file with your diagram's image. It could be open from command line by running:  

###### Ubuntu

```
nautilus diagram-definition.png
```


###### Mac OS

```
open diagram-definition.png
```

#### Convenience
Above two commands could also be joined, as a convenience command:

```
python diagram-definition.py; nautilus diagram-definition.png
```


[dac]: https://diagrams.mingrammer.com
