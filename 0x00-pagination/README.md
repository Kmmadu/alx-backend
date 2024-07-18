# ALX Backend Pagination

This repository contains projects related to backend pagination, focusing on different pagination techniques and handling large datasets efficiently. The projects are part of the ALX Backend curriculum.

## Projects

### 0. Simple Helper Function

#### File: `0-simple_helper_function.py`

This project involves writing a simple helper function named `index_range` that takes two integer arguments, `page` and `page_size`. The function returns a tuple containing a start index and an end index corresponding to the range of indexes to return in a list for those particular pagination parameters.

### 1. Simple Pagination

#### File: `1-simple_pagination.py`

This project builds on the previous task by implementing a `Server` class with a method named `get_page`. The method takes two integer arguments, `page` (default value 1) and `page_size` (default value 10). It paginates a dataset of popular baby names and returns the appropriate page of the dataset.

### 2. Hypermedia Pagination

#### File: `2-hypermedia_pagination.py`

This project extends the previous task by implementing a method named `get_hyper` in the `Server` class. The method returns a dictionary containing key-value pairs such as `page_size`, `page`, `data`, `next_page`, `prev_page`, and `total_pages`, making pagination more informative and user-friendly.

### 3. Deletion-Resilient Hypermedia Pagination

#### File: `3-hypermedia_del_pagination.py`

This project focuses on making pagination resilient to deletions. The `Server` class implements a method named `get_hyper_index`, which returns a dictionary with keys such as `index`, `next_index`, `page_size`, and `data`. This ensures that if rows are deleted between queries, the user does not miss items when changing pages.

## Setup

The project uses a dataset of popular baby names. You can find the dataset in the `Popular_Baby_Names.csv` file.

### Requirements

- Python 3.7
- Ubuntu 18.04 LTS
- `pycodestyle` style guide (version 2.5.*)

## Usage

Each project file can be tested using the corresponding main file provided in the project description. For example, to test `0-simple_helper_function.py`, you can run:

```bash
$ ./0-main.py

