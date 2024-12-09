This is the raw data used to create the [family tree of operating systems](https://eylenburg.github.io/os_familytree.htm), which is rendered using gnuclad.

Some of the dates are estimates based on e.g. the years of the project website going online and being taken down. 

If anyone can contribute corrections that will be much appreciated.

Please note that some operating systems have their end date set to the year 2100 to avoid running into a bug in gnuclad.

## Contribution guide
The ````.SVG```` file is generated from the ````.CSV```` file using the ````gnuclad```` tool.

### Installation
gnuclad can be installed via flatpack or snap.

Snap:
````
sudo snap install gnuclad
````

### How to edit the .SVG file
The CSV file can be edited with LibreOffice Calc, for example. It is important here that all lines are formatted as text when opening the CSV file in order to prevent, for example, a date from being automatically adjusted.

Once the changes have been made to the CSV file, the SVG file can be generated with the following command:
````
gnuclad file.csv output.svg config.conf
````

Example:
````
gnuclad Eylenburg_Operating_System_Timeline_Family_Tree.csv Eylenburg_Operating_System_Timeline_Family_Tree.svg Eylenburg_Operating_System_Timeline_Family_Tree.conf
````