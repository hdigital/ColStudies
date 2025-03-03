# ColStudies

ColStudies is a lightweight user interface to the  Colectica Repository API. You can see metadata for studies and register DOIs via da|ra. It uses justpy and python.

The project was inspired by the Colectica API from CLOSER, available at
<https://github.com/CLOSER-Cohorts/colectica-api>

## Changes

### Version 0.4

Added functions to manage local Files (STAR folders) and send them to DBKEdit database (GESIS specific functions).

## Usage

1) Configuration of user settings can be done in `settings.py`

2) Configuration of server settings can be done in `justpy.env`

3) To start the server, double-click on `StartColStudies.cmd`
    - basic information about status and errors are shown in the console
    - you can also use python to start the main file: colstudies.py
    - `python web/colstudies.py`

4) This will open your default browser with the start page
    - click 'reload' to refresh if it does not so automatically

5) To use ColStudies, login with your [Colectica](https://www.colectica.com/) account

## Dependencies

ColStudies uses JustPy and Python 3

Install Python dependencies with

`python -m pip install -r requirements.txt`

Pin and upgrade dependencies with

````
python -m pip install pip-tools
python -m piptools compile --upgrade --extra dev --generate-hashes pyproject.toml
```

## License

License: MIT License

Copyright (c) 2023 Wolfgang Zenk-Möltgen, GESIS
