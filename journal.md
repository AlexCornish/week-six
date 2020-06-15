## Circle of exploration
### The parts of Moravec's cycle of exploration
- Working with a limited set of information, that has messy data. 
- Deciding whether to work with messy data
- Converting it into a useable format
- Visualing the metadata
- Cleaning the data by hand
- Filtering out irrelevant information
- Creating a corpus
- Visualising the data.

- Obviously Moravec's project is leagues more in-depth than any project that could be done for a single university course such as this one, but the similarities in the cycle of exploration that digital historians take part in seems to be identical regardless of scale. 
 
### Working with a limited set of information, that has messy data.
- This is more of an inevitability than anything else, as there's likely sources for every topic that either haven't been digitised or don't exist, and given the lacking capability of the technology used in the process, the information that results from the existing sources, if not done by hand, will more likely than not have a number of formatting and general word errors. I have found this to be the case throughout this class, mainly with OCR, even the best ones, and speech-to-text.
  
### Deciding whether to work with messy data
- A critical decision that tends to involve a lot of decision making, as a lot of data tends to be messy, but in some cases can be fixed with a lot of manual work. For instance, in the chronicling america class part, I attempted to fix the text in one of the articles manually by placing the OCR output text and the chroncling america article image side by side and fixing the OCR output as I went, I only did that for one article, realised it was a lot of work and that I had 25+ other articles with the same, or possibly more problems than the one I worked on, and realised I neither had the time nor willpower to do it, nor the neccessity, I'm not really sure why I tried to do that, curiousity perhaps. In the end, I opted to work with the messy data, and was still able to get somewhat of a result with a corpus that made mostly logically sense once all of the split words, commonly reoccuring errors, incorrect characters as a result of problems to do with character encoding formats such as UTF-8 and ascii characters such as "é" (UTF-8) coming out as "Ã©" in extended ASCII. I'd say that messy data should be worked with as something important could be missed if it isn't used, however, sets should be taken, if possible to try and fix it, either by tools such as OpenRefine, or manual review, if you have enough time and/or resources. 
- Side Note: Also I did, after working with the chronclingAmerica api, try building my own tool which used multiple free-OCR engines including the slightly-outdated Tesseract made by HP in the '80s, OCRopus, and Calamari (an upgraded version of OCRopus that uses Neural networks to understand the images) and it takes the input from those multiple OCRs and compares them to one another to try and find the best match to the text which along with the use of a dictionary, which regular words can be matched to could possibly work better than using one OCR by itself. However, I have been short on time lately due to starting a new job and having 3 classes and haven't been able to work on it much. Otherwise I shall continue trying to get it to work and if you are interested, I can send you the results although I can't promise it will be any better than what already exists.

### Converting to a useful format
- Yes. I have had to do that quite a bit to varying degrees of success. Especially during the ChronclingAmerica activity, that was challenging as the free online converters had size limits or caps on how much data they would convert for you in a day before you had to subscribe to convert any more. Fortunately with a decent knowledge of code, this can be gotten around. I happen to be lucky in that what I am working for my job is fairly similar to this and I used some code that I have build for work to call an API and convert the data from XML to .csv format to make working with it easier as it's a format that works with nearly everything. Without this software, I would have been dead in the water as I couldn't get to grips with the OldBaileyOnline.org API as it's a bit weird by modern RESTful API standards. 
