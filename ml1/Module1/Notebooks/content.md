# Jupyter notebooks

Before we get with the programming assignment this week, we'll do a very brief
introduction on [Jupyter notebook](http://jupyter.org/),
which you will need for the assignment this week. These
notebooks allow a mixture of nicely formatted text and *Python* code.

Download the introduction file below.

[Right-click and save the notebook introduction file here](data/notebook.ipynb)

## Starting a Notebook server

Open your terminal in the directory where you downloaded the file, make sure
your `minai` (or `ml1`) environment is active, and run the command

    jupyter notebook

This will print some information about the *Notebook* server in the terminal,
and open a web browser to the URL of the web application. By default this is
[http://127.0.0.1:8888](http://127.0.0.1:8888). Note that *127.0.0.1* is the
home ip-address, so this is now a webpage running on your own computer!

> When this command fails with an error similar to `jupyter: 'nbclassic' is not a Jupyter command`, you can run `conda install nbclassic` to fix the problem!

This first page shows the dashboard, which lists the notebooks available in the
current directory. You can create new notebooks from the dashboard with the
`New` button (select *Python 3* notebook), or open existing ones. Creating a
new notebook will create a new file `Untitled1.ipynb`, where the extension
`.ipynb` indicates it is a notebook file.

## Running the notebook assignment

Now, using the dashboard in your web browser, open the file you saved,
which was called `notebook.ipynb`. The rest of the introduction instructions are
written in there, in the `notebook.ipynb` file.

You do not need to hand in your notebook from this short assignment, as it is
just an introduction for the programming assignment this week. Once you've
completed that, you can get started with the actual notebook assignment.
