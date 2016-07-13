# python-windows-system-tray-popup
To generate system tray popups on windows. 
This was built in Python 3.4 and please refer to the pre-requistes required for running it successfully. 
Code taken from - http://stackoverflow.com/a/15921588

Pre-requisites - 
-------
1. Python 3.4 (although it shoudn't have problem running on other Python versions.)
2. pywin32 - For people using different Python version, download .whl file from here - https://pypi.python.org/pypi/pypiwin32

Usage - 
-------
1. Save the script in your python folder. 
2. Install pywin32. 

```cmd
SET PATH=%PATH%;C:\Python34\Scripts
SET PATH=%PATH%;C:\Python34

cd C:\path #path where pypiwin32-219-cp34-none-win32.whl is saved
pip install pypiwin32-219-cp34-none-win32.whl
```
Run Python using IDLE/cmd. Run following commands on IDLE/cmd- 

```Python
import os
os.chdir('path') #path where script is saved

import systemTrayPopup
balloon_tip('Title text','Message text') #to generate system popup
```
