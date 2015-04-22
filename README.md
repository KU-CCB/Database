KU ITTC CCB Python Database scripts

#### Structure
- config.cfg     # configuration file for database scripts
- create-ccb.py  # creates the database
- update-ccb.py  # top-level database update script
- lib/           # third-party software
- plugins/       # database table update scripts (table name = script name)
- Makefile       # some useful commands
- README.md      # this readme file

##### To run the incremental updater manually:
- `python2 incremental_update_ccb.py 127.0.0.1 mysql-user mysql-pass`

##### To run the full updater manually
- `python2 update_ccb.py 127.0.0.1 mysql-user mysql-pass`

##### To clean up the directory tree (remove junk files)
- `make clean`

##### To restore up the directory tree (remove junk files and submodules)
- `make restore`
