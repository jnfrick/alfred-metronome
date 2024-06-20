# Metronome Workflow for Alfred 5.5

This is a simple python script to start and stop a metronome at whatever BPM speed you want.  

## Requirements
* Install Python 3.x
* Install pip
* Install pygame module
* Update script to point to your version of python

You'll need to update the script's hashbang to point to whatever python environment you're running on your machine.  I ended up using a virtual environment created under my home folder: #!/Users/username/.venv/bin/python

## Usage
- `met <bpm-value>` = Play metronome at specific BPM - Example: `met 60`
- `met stop`        = Stop metronome playing
- `met fix`         = In case something goes wrong, search for any instances of the script running, kill them all, and delete the temp file in /tmp

## Notes
* You'll need to update the script's hashbang to point to your python environment.  
* You need to install pip and pygame module
* If you ever have an issue or crash and metronome is still playing, you can run:  `ps aux | grep metronome.py`   to get the process ID
* Then:  `kill -9 <proc_id>`    to stop the process

