# Cryptofeed installation
 
The Cryptofeed library is intended for use by Python developers.

Several ways to get/use Cryptofeed:

* uv - `uv pip install cryptofeed`
* Git - `git clone https://github.com/bmoscon/cryptofeed`
* Zipped source code - Download [github.com/bmoscon/cryptofeed/archive/master.zip](https://github.com/bmoscon/cryptofeed/archive/master.zip)

## Installation with uv

The safe way to install and upgrade the Cryptofeed library:

    uv pip install --upgrade cryptofeed

Cryptofeed supports many backends as Redis, ZeroMQ, RabbitMQ, MongoDB, PostgreSQL, Google Cloud and many others.
Cryptofeed is usually used with a subset of the available backends, and installing the dependencies of all backends is not required. 
Thus, to minimize the number of dependencies, the backend dependencies are optional, but easy to install.

See the file [`pyproject.toml`](https://github.com/bmoscon/cryptofeed/blob/master/pyproject.toml)
for the exhaustive list of these *extra* dependencies.

* Install all optional dependencies  
  To install Cryptofeed along with all optional dependencies in one bundle:

        uv pip install --upgrade "cryptofeed[all]"

* Arctic backend  
  To install Cryptofeed along with [Arctic](https://github.com/man-group/arctic/) in one bundle:

         uv pip install --upgrade "cryptofeed[arctic]"

* Google Cloud Pub / Sub backend

         uv pip install --upgrade "cryptofeed[gcp_pubsub]"

* Kafka backend

         uv pip install --upgrade "cryptofeed[kafka]"

* MongoDB backend

         uv pip install --upgrade "cryptofeed[mongo]"

* PostgreSQL backend

         uv pip install --upgrade "cryptofeed[postgres]"

* QuasarDB backend  
  To install Cryptofeed along with [QuasarDB](https://quasar.ai/) in one bundle:

         uv pip install --upgrade "cryptofeed[quasardb]"

* RabbitMQ backend

         uv pip install --upgrade "cryptofeed[rabbit]"

* Redis backend

          uv pip install --upgrade "cryptofeed[redis]"

* ZeroMQ backend

         uv pip install --upgrade "cryptofeed[zmq]"

## Installing from source

If you wish to clone the repository and install from source, run this command from the root of the cloned repository:

    uv sync

Alternatively, you can install in 'edit' mode (also called development mode):

    uv pip install -e .

If you have a problem with the installation/hacking of Cryptofeed, you are welcome to:
* open a new issue: https://github.com/bmoscon/cryptofeed/issues/
* join us on Slack: [cryptofeed-dev.slack.com](https://join.slack.com/t/cryptofeed-dev/shared_invite/enQtNjY4ODIwODA1MzQ3LTIzMzY3Y2YxMGVhNmQ4YzFhYTc3ODU1MjQ5MDdmY2QyZjdhMGU5ZDFhZDlmMmYzOTUzOTdkYTZiOGUwNGIzYTk)
* or on GitHub Discussion: https://github.com/bmoscon/cryptofeed/discussions

Your Pull Requests are also welcome, even for minor changes.
