# Japanese-NLTK-Support
An ongoing project to make the Japanese language usable with NLTK library functions.

This project is two python files that are used together to create what is shown below. 

  - Part 1: Final Jisho Scraper
    - Comprises of the Web Scraper and the EDA and visualization for the project
    
  - Part 2: Final NLTK Support
    - Creates the functions that will assist in conditioning data to be compatible with NLTK
    
# Abstract
What this program is meant to address are the parts of the NLTK library that do not work well with Japanese text and turn them into data that can be easily used within that library. 

The program is also going to attempt to make it so that the reader/user of this does not need to be familiar with Japanese beyond the short exerpts that I provide throughout the Jupyter Notebook. While I would always recommend familiarizing yourself with the language to some extent ahead of time, I find making this as accessible as possible one of my end goals.

Below I will have listed what the project currently has completed to some degree and what are the working goals in the future. While I do have a working understanding of the language through nearly a decade of study, I am by no means a linguist, an expert translator, or know fluent Japanese. If you find an error or a better way of doing something that is shown below then by all means submit a change request and I hope that we both come out learning more from it.

## Currently Completed Goals
    - Pre-language processing
    - Basic sentence processing
    - Basic Stemming / Lemmatization
    - Particle recognition
    - Word/Character lookup and reverse lookup
    - Basic Parts of Speech Tagging
    - Basic Tokenization

## Pending Goals
    - Including more particles
    - Including complex Stemming / Lemmatization
    - Complex sentence processing
    - Stop Word inclusion
    - NER/NED inclusion
    - Better Parts of Speech Tagging
    
    
### Problems with the program
    - Verb Conjugation/Stemming has many forms but is very small amount of data
      - 5.4% of words in dataframe consist of over 75% of the rare conjugations needed
    
![Verb Tags](https://user-images.githubusercontent.com/48660919/66078624-59d78c00-e530-11e9-9192-dcce607eb55e.PNG)

    - Website used has questionable data integrity
        - Missing 'important' words (Only 6,000 words are JLPT when there should be 10,000+)
        - Specifications ignored on website (only searched for 'Common Words'
        
![JLPT Tags](https://user-images.githubusercontent.com/48660919/66078627-5ba14f80-e530-11e9-8c61-cbea2557cb1c.PNG)
![Common example](https://user-images.githubusercontent.com/48660919/66078644-62c85d80-e530-11e9-9287-b5525b64db4f.PNG)

    - Not enough Parts of Speech Tagging
      - More webscraping is required from other sites to get pronunciation, romaji, and parts of speech
      (all of which were not clear on the website scraped)
      
 # Have any suggestions or critiques?
 Please put in a commit or send me a message and I'd love to discuss anything you have to offer. This project is a labor of love and I'd like to see it through to the end but as a one person team it isn't that easy to get to a reasonable end point.
 
 Thanks for the read!
  - Jihaiku
