elasticdb
========

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview

elasticdb is a Python library for using Elasticsearch as a database. 

Installation instructions
-------------------------

    python3 -m pip install --upgrade pip
	python3 -m pip install elasticdb

## Classes
The elasticdb library has four classes:
   - `create`: creates indeces, rows, or columns
   - `retrieve`: pulls data from the database
   - `update`: changes one or more items in the database
   - `delete`: deletes indeces, rows, or columns

# retrieve

*import elasticdb.retrieve*

```python
	from elastic import retrieve
```

*retrieve has 2 methods*
   - `whole_index()`: retrieves all members of an index
   - `by_id()`: retrieves item with a specific ID

## whole_index

*request syntax*

```python

    table = retrieve.whole_index(
        ip = "0.0.0.0",
        index = string
    )

```

*parameters*
   - `ip` *(string)*: The ip of the Elasticsearch instance
   - `index` *(string)*: The index 

*response syntax*

    ```python

    {
        "id1":id1_data,
        "id2":id2_data
    }

    ```
