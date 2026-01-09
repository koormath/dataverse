<h2>Harvesting the Metadata from Datasets in Dataverse Using a Python Script</h2>

If you are using this script on the dataverse installed server where the python package are available, you could run it on the terminal.

I have prepared this document to extract metadata from datasets using Python 3.14 on Windows 11. We are using the OAI protocol to harvest the metadata.

1.	Install Python 3.14 on a Windows system
<a href="https://www.python.org/downloads/windows/">https://www.python.org/downloads/windows/</a>

2.	Add a path to Python in Environmental Variables

Eg:- <br>
  D:\Python\
  D:\Python\Scripts\

3.	Verify Installation

Open Command Prompt and run:
<br>
**python --version**

Disable Microsoft Store Python Alias, if Windows keeps redirecting Python to the Microsoft Store

Open Settings

Go to Apps → Advanced app settings

Click App execution aliases

Turn OFF:

python.exe

python3.exe

4. Restart Command Prompt and test again: <br>

**python --version**

5. Install Required Python Package** <br>
      Now install the required library: <br>
      **pip install requests**

6. Download and extract the zip file into a folder <br>

7 . Edit the **base URL** under the heading # configuration <br>
    Eg. <del>https://dataverse.harvard.edu</del>/oai </br>
    Please don't remove the /oai from the Base URL.
    Save the file as **harvest_dataverse_oai_csv.py** <br>
    
8.	Open the command prompt <br>

9.	Go to the folder where you saved the script <br>
E.g. <br>
**cd C:\Users\koormath\Documents** <br>

If the file is somewhere else, you can locate it with: <br>
**dir harvest_dataverse_oai_csv.py** <br>

10.	Run the script <br>
**python harvest_dataverse_oai_csv.py** <br>

11.	Output File <br>
It will create an output file for all metadata from all datasets. <br>
**dataverse_oai_records.csv**



