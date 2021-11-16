Introduction
***************************

With ``data-scraper`` you can scrape any website without the need of inspecting web elements or parsing HTML using Beautiful Soup etc.
With just URLs as input you get JSON data as output.
First you need to train the scraper for particular website & then run it.

It uses selenium to automate the things. You can use its inbuilt functions in a very easy way.

Installation/Usage:
*******************
You can find this package on Pypi (see `here <https://pypi.org/project/data-scraper/>`_).

Command to install :- ``pip install data-scraper``

Import data-scraper
**************************************************
.. code-block:: python

	from data_scraper import *
	
	
Train
**************************************************
It takes two URLs of 2 similiar pages to train the scraper.

**status**: True or False

**id**: id of the scraper

Here is the code:-

.. py:function:: scraper.train(link1,link2)

   
   :param str link1: First link on which scraper to run
   :param str link2: Similiar link to link1
   :return: {"status": True, "id": "Adfef343JDJSDJ"}
   :rtype: dict
   

Run
**************************************************
It runs the scraper and gives data in response.

Here is the code:-

.. py:function:: scraper.run(link1,id="Adfef343JDJSDJ")

   
   :param str link1: Link of which data to scraper
   :param str id: id of the scraper got in training
   :return: {"data1":"data1",...}
   :rtype: dict