Python-API-Connector (for Python 2.7.0)
====================

Use the https://majestic.com connectors to access web data from one of the largest web indexes available. 
The Majestic® search engine is mainly used to instantly provide Flow Metrics® which evaluate the any page on the Internet in scores between 0 and 100.
 

For set up
---------------
Clone the repository in a directory. 

Set PYTHONPATH in the Environment Variables to Python-API-connector directory. 

This will be essential as then you can import in the library from another directory.

On Windows it will be something similar to this:
```
set PYTHONPATH=C:\project\lib\Python-API-Connector;
```
On linux, in the terminal it will look something like this: 
```
export PYTHONPATH=/usr/project/lib/Python-API-Connector
```
Examples
-------------
There are a few examples of using the API-Connector in the following scripts:

* GetIndexItemInfo.py 
  * The GetIndexItemInfo command provides data on the number of backlinks to any web page or site, linking domains and the main topics for that page or web site
* GetBackLinkData.py 
  * GetBacklinkData will return rows of data with information about all the pages linking to a given URL or domain
  
The follwoing code is from GetIndexItemInfo.py, it will shows how the API-Connector can be used.
```
api_service = APIService(app_api_key, endpoint)
response = api_service.execute_command('GetIndexItemInfo', parameters)
```



Further notes  
------------------
The Python Connector has been developed using Python 2.7.2.\
To run the examples have python 2+ installed, then in terminal use ```>python2 somefile.py```  
This will run the script or try ```py``` to run the file.



For further information see api documentation @ https://developer-support.majestic.com/


