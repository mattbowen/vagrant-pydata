Installation
============

* Install `virtual box <https://www.virtualbox.org/wiki/Downloads>`_
* Install `vagrant <https://www.vagrantup.com/downloads.html>`_
* Clone this repo: ``git clone https://github.com/mattbowen/vagrant-pydata.git``
* Install ansible (preferrably in a virtual environment): ``pip install ansible``
* Run ``vagrant up`` in the directory where you cloned the repository
* Find something else to keep you busy for the next 30-45 minutes
* Run ``vagrant ssh`` when the box is finished setting itself up

Usage
=====

Out of the box, you'll have what should be all the packages you need for doing data analysis in python, including
pandas, ipython notebook, BeautifulSoup, and scikit-learn. See the
`base requirements file for details. <provisioning/templates/requirements.txt.in>`_

To start doing data analysis, you can start a new project by typing ``mkproject <project_name>`` at the shell. This
will create a new environment with all your dependencies in it and create a folder for your project's files. Then, to
startup ipython notebook for a given project, run ``notebook <project_name>``. This will startup ipython notebook on
`http://localhost:8888 <http://localhost:8888>`_. It will also create a "notebooks" directory for your project.
