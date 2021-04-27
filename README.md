# Econ N Metrics

A project for Stanford's COMM 277T course.

## Usage

To run the website for development, navigate to the `site/` directory
and fire up a python web server:

```
cd site
python -m http.server
```

Then go to http://localhost:8000 and navigate to appropriate page(s).

> It's important to use the web server because using any external JS
> requires serving the data in the same way as you would in a production
> setting on the web. If you try to access the HTML file using your
> browser with the `file://` scheme (i.e. without the web server),
> you will get Cross-Origin (aka CORS) errors when trying to access
> "local" JSON files.


## Scrum Meetings
Scrum meetings are held daily from 4PM-4:15PM PST.

## SMART Goals

### Rachel

By the last week of the quarter, I will produce a user-friendly website that has a landing page with a search bar, and a detail  page with a nav bar/tabs and interactive data visualizations. This dashboard/web application will serve as a tool for local reporters to understand their area’s economic health. I hope to gain some skills in data gathering/wrangling, but I hope to mostly focus on creating interactive data visualization and designing/developing a UX-friendly website (even if it’s simple).

### Michael
By the last week of the quarter, I will support development of a user-friendly website and produce at least two static charts and two interactive data visualizations within this website by sourcing and analyzing relevant local-economic data. The backend analysis, data-sourcing and data visualizations will help feed into my team's interactive website/dashboard, which is meant to support local journalists in understanding their area's economic health. In achieving this goal, I hope to learn and develop basic front-end and back-end data-storytelling skills, which will ultimately help me better communicate data to a wider audience.

Key skills I hope to develop include:
- HTML
- CSS
- Javascript

## Setup

> Before using this project, please ensure all dependencies are installed. See the [project home page][] for details.

[project home page]: https://github.com/stanfordjournalism/cookiecutter-stanford-progj#requirements--setup

After creating this project, if using Python:

* `cd bna-econ-n-metrics`
* `pipenv install`

To run Python, it's recommended to do so in the virtual shell. Start with:

* 'pipenv shell'

## Installing Python libraries

```
cd bna-econ-n-metrics
# Install one or libraries, e.g. requests and BeautifulSoup
pipenv install requests beautifulsoup4
```

## Files & Directories

Below is an overview of the project structure. It is subject to change as the project develops, but will be updated regularly:

```   
├── Pipfile
├── Pipfile.lock
├── README.md
├── data
│   ├── processed (Raw data that has been transformed)
│   └── raw (Copy of original source data)
├── lib (Re-usable Python code in .py files)
│   ├── __init__.py
│   └── utils.py
├── notebooks (Jupyter notebooks)
├── scripts
│   ├── analysis (Analyze data for templating)
│   ├── data_wrangling (Source and clean data for analysis)
│   ├── templates (html templates to be used in Jinja rendering)
├── site
│   ├── county-data (HTML files for each county)
│   └── static
│       ├── CSS
│       └── JS
└── tasks (Invoke task definitions)
    ├── __init__.py
    └── code.py

```

## Reference

* [Hitchhiker's Guide to Python](https://docs.python-guide.org/)
* [Python Standard Library](https://docs.python.org/3.7/library/index.html). A few especially useful libraries:
  * csv - reading/writing CSV files
  * json - reading/writing JSON
  * os - working with OS, e.g. getting environment variables and walking directory/file trees


[BeautifulSoup]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
[invoke]: https://www.pyinvoke.org/
[jupyter]: https://jupyter.org/
[matplotlib]: https://matplotlib.org/tutorials/introductory/usage.html#sphx-glr-tutorials-introductory-usage-py
[pandas]: https://pandas.pydata.org/pandas-docs/stable/
[pipenv]: https://pipenv.readthedocs.io/en/latest/
[requests]: https://2.python-requests.org/en/master/
[selenium]: https://selenium-python.readthedocs.io/
