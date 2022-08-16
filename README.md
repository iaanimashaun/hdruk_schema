# hdruk_schema

This project checks if metadata uploaded to hdruk gateway conforms to hdruk schema 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development.

### Prerequisites

These are the requirements required for the project to be deployed. This includes


```
pandas==1.4.3, termcolor==1.1.0, validate_email==1.3, validators==0.20.0
```

These are in the requirements.txt

### Installing

A step by step series of examples that tell you how to get a development env running

Get a copy of the repo
```
git clone https://github.com/iaanimashaun/hdruk_schema.git
```


(Optional) Create a virtual environment. We have used conda here, however, you can use alternatives like vierual env or poetry. 
```
conda create -n env
```


Install required dependencies
```
pip install hdruk_schema
```





## Usage

Import necessary package
```
from hdruk_schema.schema_validator import parse_json_file, schema_validator
import pandas as pd
```

Load metadata and schema
```
metadata_filepath = 'path/to/datasetsv2.json'
schema_filepath = "path/to/datasetschema.json"

df = parse_json_file(json_filepath)
```

```
result = schema_validator(json_filepath, schema_path)
```


## Built With

* [validators](https://github.com/kvesteri/validators) - Python data validation for Humans e.g used to validate url
* [validate_email](https://github.com/syrusakbary/validate_email) - Validate_email is a package for Python that check if an email is valid, properly formatted and really exists.
* [termcolor](https://pypi.org/project/termcolor) - ANSII Color formatting for output in terminal. Used to change text color




## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

<!-- ## Acknowledgments -->

<!-- * Hat tip to anyone whose code was used
* Inspiration
* etc -->

