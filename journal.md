## Circle of exploration
### The parts of Moravec's cycle of exploration
- Working with a limited set of information, that has messy data. 
- Deciding whether to work with messy data
- Converting it into a useable format
- Visualing the metadata
- Cleaning the data by hand
- Filtering out irrelevant information
- Creating a corpus
- Explore the data.

- Obviously Moravec's project is leagues more in-depth than any project that could be done for a single university course such as this one, but the similarities in the cycle of exploration that digital historians take part in seems to be identical regardless of scale. 
 
### Working with a limited set of information, that has messy data.
- This is more of an inevitability than anything else, as there's likely sources for every topic that either haven't been digitised or don't exist, and given the lacking capability of the technology used in the process, the information that results from the existing sources, if not done by hand, will more likely than not have a number of formatting and general word errors. I have found this to be the case throughout this class, mainly with OCR, even the best ones, and speech-to-text.
  
### Deciding whether to work with messy data
- A critical decision that tends to involve a lot of decision making, as a lot of data tends to be messy, but in some cases can be fixed with a lot of manual work. For instance, in the chronicling america class part, I attempted to fix the text in one of the articles manually by placing the OCR output text and the chroncling america article image side by side and fixing the OCR output as I went, I only did that for one article, realised it was a lot of work and that I had 25+ other articles with the same, or possibly more problems than the one I worked on, and realised I neither had the time nor willpower to do it, nor the neccessity, I'm not really sure why I tried to do that, curiousity perhaps. In the end, I opted to work with the messy data, and was still able to get somewhat of a result with a corpus that made mostly logically sense once all of the split words, commonly reoccuring errors, incorrect characters as a result of problems to do with character encoding formats such as UTF-8 and ascii characters such as "é" (UTF-8) coming out as "Ã©" in extended ASCII. I'd say that messy data should be worked with as something important could be missed if it isn't used, however, sets should be taken, if possible to try and fix it, either by tools such as OpenRefine, or manual review, if you have enough time and/or resources. 

### Side Note: 
Also I did, after working with the chronclingAmerica api, try building my own tool which used multiple free-OCR engines including the slightly-outdated Tesseract made by HP in the '80s, OCRopus, and Calamari (an upgraded version of OCRopus that uses Neural networks to understand the images) and it takes the input from those multiple OCRs and compares them to one another to try and find the best match to the text which along with the use of a dictionary, which regular words can be matched to could possibly work better than using one OCR by itself. However, I have been short on time lately due to starting a new job and having 3 classes and haven't been able to work on it much. Otherwise I shall continue trying to get it to work and if you are interested, I can send you the results although I can't promise it will be any better than what already exists.

### Converting to a useful format
- Yes. I have had to do that quite a bit to varying degrees of success. Especially during the ChronclingAmerica activity, that was challenging as the free online converters had size limits or caps on how much data they would convert for you in a day before you had to subscribe to convert any more. Fortunately with a decent knowledge of code, this can be gotten around. I happen to be lucky in that what I am working for my job is fairly similar to this and I used some code that I have build for work to call an API and convert the data from XML to .csv format to make working with it easier as it's a format that works with nearly everything. Without this software, I would have been dead in the water as I couldn't get to grips with the OldBaileyOnline.org API as it's a bit weird by modern RESTful API standards. 

### Visualising the Metadata
- Didn't do that for the final week, although I'm assuming its like that week with the civil war letters, kind of looking at the interactions between people in networks. However, if using charts in R counts, then I did that.

### Cleaning the data by hand
- As mentioned before, I've done this in the original corpus and in this final week, by formatting the data into a better formatted .csv file with separate columns for the date of the trial, the verdict, the sentence, and the description of the trial. Other than that, I was fortunate that the data source that I'd chosen had taken great efforts to provide accurately transcribed data. Also I liked that in her presentation, Moravec gave credit to her assistant who did all of the work in cleaning up the data by hand and I hope recognition like that is more prevalent nowadays than it was in the past.

### Filter out irrelevant Information
- One of the main benefits of digital history is that it makes it a lot easier to filter out information that isn't relevant, in Moravec's case, in mentioning the women in Schneemann's letters, she mentions that 5 of them are mythical and/or fictional, and those can be filtered out using the technology to focus on those who exist. I too filtered irrelevant information in this week's work with me filtering out every terms, using the word omitting feature in Voyant, that wasn't related to an object that could feasibly be stolen by a highway robber, I did this until I ended up with a shortlist of about 20 terms, each of which appeared at least 10 times across the 99 trials. This left me with the words appeared in case and for the most part related to items that had been stolen during highway robberies. 

### Create a Corpus:
- The corpus I used for the center part of the poster was the original corpus before the filtering of irrelevant information relating to the stolen items part that interested me for some reason, in retrospect, not quite sure what, but the theft of clothing was something I hadn't expected to be a major part. The corpus is good for highlighting certain words that would be expected to be present such as prisoner, took, and robb'd. However, it is also useful in finding words that one might not expect to find in such a circumstance. As I had no idea about the justice system at this time, I was surprised to see about Juries and Prosecution, even in the smaller cases.

### Explore the data:
- After the process, I was able to explore the data in a number of ways. By looking at the corpus to see what stood as unusual, by collecting the data and creating charts to demonstrate it, and by filtering the data using voyant to find out about the most commonly stolen items were. From that I was able to determine what the most commonly stole items were, what kind of punishments they were likely to face, and how often those accused were guilty, along with finding out some information about the judicial system at the time. 

As for continuing the cycle, this process did raise a couple of questions such as, what were the differences between these type of crimes for men and women, such as did men typically take different things, were they more or less often guilty of what they were accused, did the kinds of punishments they would get differ, and what kind of words appear on the male corpus that don't appear on the female ones. Similarly, this process also made me wonder how these questions about highway robbery (guilty or non-guilty, punishment received/ what was taken) compared to other kinds of robberies done by women during the same time, which would be interesting with the highway robbery being a small part of a larger scale project created by the expanding scope caused by the cycle of exploration. 
