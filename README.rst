====
Project Title
====

This is a 2 to 3 sentence description about the project. It doesn't need to be too detailed; just enough to give a high-level overview of the solution. Detailed documentation may be linked at the **Additional Documentation** section of the README.


Usage
====

Developing
----

Prerequisites
~~~~

Tools
++++

* Python; >= 3.8, < 3.10
* Node.js; >= 16.17
* Docker

Servers
++++

* Postgres
* Redis
* ZMQ

External Services
++++

* Databricks
* Google Firebase

Setup
~~~~

Clone
++++

Clone the repository to the local development machine.

::

    $ git clone git@github.com:project/repository.git
    $ cd repository

Environment
++++

Create a virtual environment (for Python).

::

    $ python -m venv .venv
    $ source .venv/bin/activate
    (.venv) $ python -m pip install -U pip
    (.venv) $ python -m pip install -r requirements.txt

Configure
~~~~

Setup the environment variables.

::

    (.venv) $ touch .env
    (.venv) $ echo 'DB_URL=postgres://username:password@localhost:5432/dbname' >> .env
    (.venv) $ echo 'FIREBASE_API_KEY=blah-blah-blah' >> .env

Run
~~~~

Run the code.

::

    (.venv) $ python app.py

Deploying
----

Package
~~~~

Create bundle or compile the application *(if needed)*.

::

    (.venv) $ python -m pyinstaller app.py

Or build a Docker image and push to the remote container registry.

::

    (.venv) $ docker build -t project/app:version .

CI/CD
~~~~

* Ensure that the CI/CD YAML file is updated
* Push code to remote to trigger CI/CD based on the rules set in the service provider

Additional Documentation
====

These are additional detailed documentation for the project located at:

* the ``/docs`` folder of the repository
* the external knowledgebase like JIRA Confluence or Google Docs