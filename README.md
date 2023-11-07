# offlineinstaller-python101
offline installer for critical python packages

Built for `win10` or `win11`

## Instructions

1. Create requirements using `venv`

   ```powershell
   python -m venv venv
   .\venv\Scripts\activate
   pip install .. .. .. 
   pip freeze > requirements.txt
   ```
   
1. Download as offline packages
 
   `pip download -r requirements.txt`

1. On the offline system, use `pip install --no-index --find-links /path/to/download/dir/ -r requirements.txt`

   ```powershell
   git clone https://github.com/jakelime/offlineinstaller-python101.git
   cd offlineinstaller-python101
   pip install --no-index --find-links . -r requirements.txt
   ```
