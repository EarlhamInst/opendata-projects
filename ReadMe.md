

A script to import the metadata from a json file into the iRODS server


## Installation

```
python3 -m venv venv

```

```
source venv/bin/activate
pip install python-irodsclient
```


## Usage

```
usage: import_projects.py [-h] [-i INPUT_FILE] [-H HOST] [-P PORT] [-u USER] [-p PASSWORD] [-z ZONE]
                          [--uuids [UUIDS ...]] [-v]

options:
  -h, --help            show this help message and exit
  -i INPUT_FILE, --input_file INPUT_FILE
                        The input Projects JSON file to load
  -H HOST, --host HOST  The iRODS server hostname
  -e ENV_FILE, --env_file env_file  The iRODS environment json file to get the host, user, zone and port from if you would prefer to set the arguments that way
  -P PORT, --port PORT  The port that the iRODS server is running on
  -u USER, --user USER  The username to use to log in to the iRODS server
  -p PASSWORD, --password PASSWORD
                        The password to use to log in to the iRODS server
  -z ZONE, --zone ZONE  The iRODS zone to connect to
  --uuids [UUIDS ...]   The Project UUIDS to parse. If this is not set, all projects in the file will be parsed.
  -v, --verbose         Display progress messages
```
