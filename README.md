# :newspaper: Word Hunter  
  
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  *- Automated online Treasure hunt*  

## Description  
***Word-Hunter***  is a question suggester for [Online Treasure Hunt](https://en.wikipedia.org/wiki/Online_treasure_hunts "Online Treasure Hunt") games (i.e .. this automatically prepares clues using online searches extensively) . All you'll have to do is to give it a **Topic of Interest** , and it'll search for different words relating to the topic and automatically set a question based on the frequency of words and other factors .  
___  

## Demonstration

[![asciicast](https://asciinema.org/a/eitugvhnhrbf6xzny20c92wdq.png)](https://asciinema.org/a/eitugvhnhrbf6xzny20c92wdq?autoplay=1)  

.... and here is what your question would look like :  
![sample_wh](https://cloud.githubusercontent.com/assets/10980285/16002397/104cee9e-3175-11e6-8361-2a3b599bba71.png)  


##### Explanation
- ``` MVC ``` and ``` development ``` are word clues  
	* It gives us an idea that the answer could be a MVC framework  
- The visual clue is the picture of a ``` Flask ```  
	* At this point , the visual clue doesn't make much sense  
- On hovering over the picture , the title ``` Python ``` pops up  
	* Alas , all of these words , ``` MVC , development , Flask , Python ``` seem to make sense !  
		- Hence the final answer has to be a python MVC framework , which is ``` Django ```  

___


## Specifications  
* OS : All Linux distributions  
* Core language : python 2.7.x   

___  

## Tools used  
* [Google custom search API](https://developers.google.com/custom-search/ "Search API") (For both images and words)  

> Please note that , using the **google custom search API** , you can make only 100 calls per day   
> and currently , 8 calls are made per execution  


* [google-api-python-client](https://pypi.python.org/pypi/google-api-python-client/)  
* [Beautiful Soup 4](https://pypi.python.org/pypi/beautifulsoup4 "Beautiful Soup")  
* [NLTK python](http://www.nltk.org/ "Natural language tool kit python")  
* [urllib2 python](https://docs.python.org/2/library/urllib2.html)   

___  

## Benefits  
> This can easily be implemented on any python server (To host similar competitions) .  
> You can also extract out some kind of a suggestion in the form of words , in case you're setting questions for an online treasure hunt competition .  


## Running the app  
``` $ git clone https://github.com/shravan97/WordHunter ```  
``` $ cd WordHunter ```  
``` $ python wordhunt.py ```  
___  


## ToDo  

- [ ] Include a loading bar , when the fetched URLs are being scrapped and when frequency is being calculated  
- [ ] Better way to filter out the massive amount of noise that comes along with search words  
- [x] Add pictures and gifs of a sample execution  
- [ ] Better word suggester (Both interms of filtering and its frequency)  
- [ ] Search term used for image search needs to be automatically found  
- [ ] Implement multiprocessing in parts which are slower to run  
- [ ] Program will have to terminate smoothly on keyboard interrupts and other hindrances  
- [ ] Instead on taking a topic everytime as input , try taking in as a bunch initially and print questions with a random topic of interest  
- [ ] Give weightage to the page on which the search result appears on querying  

___  


## Contributing  
Got any cool idea that could be implemented here ? Go ahead and give a pull request . Or You may as well put it up as an issue [here](https://github.com/shravan97/WordHunter/issues "Issues") . Please read [this](https://github.com/shravan97/WordHunter/blob/master/CONTRIBUTING.md) document here for more details about contributing  


[Please don't forget update the contributors' list below when you're giving a pull request :smile: ]
___  

## Contributors  
* [shravan97](https://github.com/shravan97)  

																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																			