# Best practices in data visualization

https://python.g-node.org Summer School 2015

https://python.g-node.org/wiki/schedule

## Setup

We run [Python 3](https://www.python.org/) as in the rest of this Summer School.
We use [virtual environments](https://virtualenv.pypa.io/) as a general good practice.
Python 3 ships with `virtualenv` but, on Ubuntu 14.04, initiating a virtual environment with

    $ python3 -m venv ~/.virtualenv/gnode-datavis

errors, so I had to use

    $ virtualenv --python=python3.4 ~/.virtualenv/gnode-datavis

As you can see, I tend to keep (all) my virtualenvs under `~/.virtualenv`; adapt to your own tree and practices.

    $ source ~/.virtualenv/gnode-datavis/bin/activate
    $ pip install --upgrade pip

Install all the Python packages used in this course:

    $ pip install -r requirements.txt

I wanted to run the dev version of `matplotlib`, so I did:

    $ cd ~/python
    $ git clone git@github.com:matplotlib/matplotlib
    $ cd matplotlib
    $ pip install .

If you prefer running a stable version, feel free to

    $ pip install matplotlib==1.4.3

Launch the Jupyter Notebook, [formerly](http://blog.jupyter.org/2015/04/15/the-big-split/)
known as the IPython Notebook:

    $ jupyter notebook
