# cookiecutter-snakemake

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


## Snakemake directory structure
A simple `Snakemake` file consists of several rules and Python functions to
execute workflows.  With large workflows, however, the enter pipeline file can
be cumbersome and difficult to maintain.  `Snakemake` has a recommended
structure to simplify large scale workflows by seperating it into common
rule and function files.

The `Snakemake` structure was obtained from the [snakemake deployment](https://github.com/snakemake/snakemake/blob/fdc26e642f08fb4ca3f66fe8e310e8eda8a954a6/docs/snakefiles/deployment.rst)
documentation.

```
├── README.md
├── workflow
│   ├── envs
|   │   └── environment.yaml
│   ├── rules
|   │   └── common.smk
|   │   └── defaults.smk
|   │   └── rule.smk
│   ├── scripts
|   │   ├── script1.py
|   │   └── script2.R
|   └── Snakefile
└── config
    ├── config.yaml
    └── some-sheet.tsv
```


## Installation
Install the latest version of `cookiecutter` if you have not already.
```
pip install cookiecutter
```


## Usage
Generate the `snakemake` project using `cookiecutter`:
```
cookiecutter https://github.com/simpsonlab/cookiecutter-snakemake.git
```
Several items will be requested which will be used to complete the template
files and directories:
```
name [project]: project_name
author [Author Name]: Simpson Lab
institute [Institute Name]: The Ontario Insitute for Cancer Research
year [2020]:
```

A directory with the name `project_name` will be created and default files and
sub-directories will be constructed as described above.


## Credits and Acknowledgements
The initial boilerplate setup was influenced by (https://github.com/audreyfeldroy/cookiecutter-pypackage).


## License
MIT
