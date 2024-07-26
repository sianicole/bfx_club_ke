You can install all the tools in one environment by using an environment file `yaml file`, a configuration file used to define and create environments.YAML files, when used with tools like Conda or Docker, help manage dependencies to prevent conflicts between installed tools within an environment. This enables you to set up all the necessary tools for a specific analysis in one stable environment, ensuring ease of scripting and reliability. Pretty cool huh!😎
## How to create a yaml file
### Open a text editor e.g Notepad
### Write yaml content
An example of a yaml file can be found [here](https://github.com/sianicole/bfx_club_ke/blob/main/bfx-club.yml))
### Save the file
1. Click on File in the top menu.
2. Select Save As.
3. Choose the location where you want to save the file.
4. In the "Save as type" dropdown, select "All Files".
5. Name your file with a .yaml or .yml extension (e.g., file-name.yaml).
6. Click Save.
### Use the yaml file to set up your environment:
Make sure you are in the directory containing the yaml file then run the code below:
```
conda env create -f <file-name>.yml
```
