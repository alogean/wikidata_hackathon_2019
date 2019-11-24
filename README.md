# Wikidata Hackathon 2019
## Some informations
- Repository used to manage information and code created during the wikidata hackathon of Nov. 2019 https://github.com/WikidataZurichMeetup/meetup-1
https://www.wikidata.org/wiki/Wikidata:Events/Wikidata_Zurich_Hackathon2019
- Cristina Sarasua (Uni Zurich)
- Ilario Valdelli

## Corpedia
We build a portal about companies. 
There are around 300'000 companies in Wikipedia/Wikidata.
see here https://www.wikidata.org/wiki/Wikidata:WikiProject_Companies

how to use a python bot
https://github.com/opendatazurich/wikidata-training/blob/master/Wikidata%20-%20Create%20a%20new%20bot.ipynb

Corpedia Frontend Repo: https://github.com/Tamalera/compedia
SPARQL in Python: https://github.com/opendatazurich/wikidata-training/blob/master/Wikidata%20SPARQL%20Query.ipynb

https://codepen.io/alogean/pen/ZEEZdwN

https://github.com/tak2/compedia_backend

https://www.wikidata.org/wiki/Wikidata:Pywikibot_-_Python_3_Tutorial/Data_Harvest

https://threejs.org/examples/#webgl_buffergeometry_drawrange

webapi call
https://www.wikidata.org/w/api.php?action=wbsearchentities&search=novartis&format=json&language=en&uselang=en&type=item

Webapi help
https://en.wikipedia.org/w/api.php

Zurich, Switzerland
Direct: +41 43 285 67 81 Mobile: +41 79 351 84 82 Email: Antoine_Logean@swissre.com
 
 
News volume
1.     https://api.gdeltproject.org/api/v1/search_ftxtsearch/search_ftxtsearch?query=insurance&output=timeline&outputtype=vol&timelinesmooth=5
To shows list of news articles in English language
2.     https://api.gdeltproject.org/api/v1/search_ftxtsearch/search_ftxtsearch?query=insurance&output=artlist&dropdup=true&trans=googtrans
To show list of news articles in English + Images
3.     https://api.gdeltproject.org/api/v1/search_ftxtsearch/search_ftxtsearch?query=insurance&output=artimglist&dropdup=true&trans=googtrans
4.     Country Filer +  new article list + translated
https://api.gdeltproject.org/api/v1/search_ftxtsearch/search_ftxtsearch?query=sourcecountry:india&output=volume&sort=desc&trans=googtrans

def getqfromurljson(corpname):
    urlc = "https://www.wikidata.org/w/api.php?action=wbsearchentities&search="+ quote(corpname,safe='/:?=&') +"&format=json&language=en&uselang=en&type=item"
    #print(urlc)
    with urllib.request.urlopen(urlc) as url:
        data1 = json.loads(url.read().decode())
        name = extract_values(data1, 'id')[0]
    return name
    
for getting all the data
https://www.wikidata.org/w/api.php?action=wbgetclaims&entity=Q26463
for a specific property
https://www.wikidata.org/w/api.php?action=wbgetclaims&entity=Q26463&property=P17

to decode the qcode
https://www.wikidata.org/w/api.php?action=wbgetentities&ids=Q148&props=labels&languages=en&format=json

to decode multiple qcode use |
https://www.wikidata.org/w/api.php?action=wbgetentities&ids=Q148%7CQ72&props=labels&languages=en&format=json


## Other ideas

### Wiki-Sense

### GDELT

### Critical Infrastructures

### Cyber Loss Modeling 

