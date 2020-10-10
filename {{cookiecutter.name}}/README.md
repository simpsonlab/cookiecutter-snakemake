# {{cookiecutter.name}}

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



## Usage



## Credits and Acknowledgements


## License
MIT
