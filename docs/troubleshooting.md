# Troubleshooting

This article discusses how to troubleshoot the job search agent. 

## Using the correct version of Python

JobSpy doesn't yet run on Python 3.14. You need Python 3.12 to run it. If you have more than one version of Python on your machine, use the following command: 

```python

python3.12 job_search.py

```

## LinkedIn Skips a Search Term

Don't worry if LinkedIn skips a search term. The job search agent will still run.

## No Results Collected

No results collected can mean the following things: 

- your internet dropped during the run
- JobSpy blocked the results (they do this occasionally)
- a JobSpy update broke something

Wait a few hours before running the job search agent again. 

## Script Fails to Run

When the script fails to run, the following things may be happening:

### Before the job search agent runs

- you're using the wrong Python version
- you didn't install JobSpy under Python 3.12
- there are syntax errors in the script through improper copying and pasting

## While the job search agent runs

- LinkedIn returns a job listing from an unsupported country/region.
- Indeed or LinkedIn temporarily blocks the scraper for making too many requests too fast
- your internet drops mid-run

## CSV Opens as Raw Text

The `.csv` file can open in a text editor, which causes the data to display as raw text. To view it in table format, be sure to open the `.csv` file in Excel, Numbers, or Google sheets. 