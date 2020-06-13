# Week Six Notes

## Readings

### http://historyinthecity.blogspot.com/2013/11/before-i-start-i-want-to-thank-people.html
- *"Feminist Artists and Network Analysis"* : This seems like a really interesting topic to explore and analyze... I can see how the tools we have learned about over the last few weeks would enhance this venture.
- *"corpus linguistics might reveal interesting aspects of her as female artist in a largely male milieu."* : a reoccurring theme in our studies...
- I do not fully understand that first vizualization but I can appreciate the complexity and odd beauty of it. It seems to be a timeline of sorts. 
- The following breakdown of simpler vizualizations definetly make more sense and give more insight as to what the author is trying to explore.
- I really liked how she broke down her process of analyzation. It was especialy cool that I now recognize most of the tools and concepts mentioned.
- I wont lie, I was actually impressed that I understood most of what she was saying. It really shows how much I've learned over these past few weeks. The included vizualizations helped alot as well.
- Her text ends in a question: *"I also really wanted to talk about data visualization as a tool in DH.  The above two images show the same data represented two ways.  The lower is Gephi, the "hot" tool of network analysis, while the top is the relatively easy to use Raw interface.  Which seems clearer? "*
    - To answer this I have to say the first vizualziation, made through raw, is more clear to me. Even tho upon first glance it seems more complex due to all the extra "parts" it is easier to read because there is not much to interpret. The lines show direct correlations, where as the "network diagram" (of sorts) is more messy and up to interpretation to me.
    
# Final Task

### What source did I choose?

**Instructions:** Remember back in week one, how I had you explore that twitter thread by Amalia Skarlatou Levi? This week, you’ll be selecting one of those resources she shared (or, if none strike your fancy, something from the resources gathered here) to do some exploratory digital history.

From the "Diary Index" (https://diaryindex.com/digitized-diaries/) provided, I have selected Claire Eva Paine's Diary (https://www.kansasmemory.org/item/228565) to explore and analyze. I can not exactly put my finger on why, but It seemed interesting to explore something I have virtually no knowledge about. I find it interesting that she is not a major "historical figure" and from first glance, the book is mearly her simple day to day thoughts as an average working woman. I will see if I can find any patterns in her enteries.

### What will I do with my source?

**Instructions:** You will use at least three appropriate techniques from weeks 1 to 4 to identify and surface some interesting historical observations from those sources, and you will imagine the possible directions such research might take.

Much like the reading we did for this week, I think my main goal will be to download her diary (either the images or the already inscripted text available), clean the text up and then analyze and interpret it using various tools to see if there are any patterns that can be visualized. 

## **Step 1: Downloading the Text using WGET and PYTHON**

- I was having difficulty at the beginning and getting a whole bunch of error messages, but after refering back to my week one notes, I realize now that the "wget.exe" file needs to be in the directory that I am downloading things into. I am hoping this works...
- An improvement... It did download but not how I wanted it to... I think it has something to do with the URL. I will try something else.
- Its odd, I felt I followed the steps but no matter what I did it seems to not download the individual images but made an index page of sorts? I have attached pictures of my attempts.

**This is the link of the first journal page/what I assumed was directory:**

![issue](https://github.com/Elissap5100/Week-Six-Work/blob/master/Wget%20Issue/IssueA.PNG)

**This is the code I used to (unsuccessfully) download the images:**

![issue](https://github.com/Elissap5100/Week-Six-Work/blob/master/Wget%20Issue/IssueB.PNG)

**I included the "index" page HTML code that was created during my first attempt for curiosity sake in the repository in a folder titled "www.kansasmemory.org/item/228565".

- Both attempts did not work, but fortunately the text version of the entire diary is available, so I decided to use that and clean it up. It just would have been nie to successfully download the imaes and maybe transcribed the text myself using an OCR technique. 

**UPDATE** : It let me download a single image using the direct URL of the image, not the website directory as our class instructions indicated. Here is the URL that worked: https://img.kansasmemory.org/00397683.jpg. I am afraid to try but maybe I will attempt the beginning part of this URL... and hopefully it won't download the entire website?
        - That did not work... but I realize now I have to follow the next part of the lesson titled "Using python to generate a list of urls" and "Using wget with a list of urls". I will do that now and see what happens!
        
**Update 2:** It worked! Evidence will be in the repository (and the rest of this project) but here is a picture of the code used!
*I am unsure why I exactly needed all the journal images, but I think I just wanted to prove to myself I could do it. Plus, it is better safe than sorry to have the reference images incase I can't understand some of the transcribed text available.*

![issue](https://github.com/Elissap5100/Week-Six-Work/blob/master/Wget%20Issue/Resolved.PNG)

## Step 2: Clean the Text with REGEX
- This step is a bit harder to show, but using various REGEX commands from both pur course and online resources (which will be linked shortly), I cleaned up the text of any major errors in text or added labels (I removed the page numbers, blank page indicators, the header and footer labels, copyright instructions, etc). I knew this was formatted like the other data we looked at for this portion of our week 3 lessons, so I did not feel the need to organize the data in a way that it would work easily with open refine.
- Resources that helped me for this step included:
        - https://craftingdh.netlify.app/week/3/regex/
        - https://stackoverflow.com/questions/41489818/in-sublime-text-3-is-there-a-shortcut-to-remove-blank-lines-in-a-selected-text
        - https://github.com/NicholasBuse/sublime_DeleteBlankLines
        
- The Original and New txt files will be located in a folder in the repository named "textfiles".
- I wanted to use networks, but I quickly learned (as the lesson plan stated) that this was a time where a network analysis was not appropriate. 
- The more I explore the writing in this stage, I learned that many of her ramblings really just are ramblings. There are also many blank days (as stated by the original source). Upon first glance there does not seem to be any major narrative. There are a few names which appear often, but that is to be expected. In the next steps, I am hoping to find ome major themes or thoughts throughout her year.
        
## Step 3: Text Analysis with Voyant
- This is the step I was most looking forward to! I hope to try at least 2 different ways to analyze the text from her diary, and see if there are any patterns or recurring topics.

- Upon first glance with no filtering options, the most used words are typically names of people in her life. I will attempt to explore the context of these names and see who these people are to Claire.
```
Most frequent words in the corpus: 1942 (330); tom (216); annie (100); don (86); evening (78)
```

![CloudA](https://github.com/Elissap5100/Week-Six-Work/blob/master/Voyant%20Findings/CommonWords.PNG)

- Here is the unflitered word cloud:

![CloudA](https://github.com/Elissap5100/Week-Six-Work/blob/master/Voyant%20Findings/A1.PNG)

- After playing around with the various filters and exploring the different contexts in which each of the names are used in I fel confident about the following statements:
    - Tom is Claire's husband or brother( I am honestly unsure), who is in the army and leaves once or twice for training. Although he seems to stay in contact through letters to their family.
    - Ruth is mentioned often but I am unsure her role. Perhaps a simple friend? or maybe Tom's wife?
    - Annie is Claire's sister who she lives with
    - Don is Claire's brother, an optometrist, who she worked as an assistant for
    
- After further analysis of the entries I found there was no explicit them really, but Claire was a woman with deep connections and care for her friends and family, especially Tom, who are in her life. 
- Everytime I would move things or take out works or filter the data, it seems names, such as Tom, annie, Bill, Don and more would always be the most prevalent topics in her texts. 

![CloudB](https://github.com/Elissap5100/Week-Six-Work/blob/master/Voyant%20Findings/B1.PNG)

- I am unsure if it can be done easily, but Tom often wrote letters to Claire about his movements and where he would be placed within the military. For the ext part of this project, I may attempt a story map documenting his movement. This following screenshot shares moments from when he would send letters to claire, typically which included where he was at that point and time:

![CloudB](https://github.com/Elissap5100/Week-Six-Work/blob/master/Voyant%20Findings/Tommove1.PNG)

![CloudB](https://github.com/Elissap5100/Week-Six-Work/blob/master/Voyant%20Findings/Tommove2.PNG)

- Overall, I am happy with what Voyant has taught me about this text, as well as introducing me to a plan I can hopefully move forward in for the next part of this assignment. It allowed me to analyze topics that appeared more heavily than others and learn more about what was important to Claire.

You will share your results using an appropriate technique you encountered in week 5. Other possibilities are ok too; just check with Dr. Graham first. Remember, you don’t have a lot of time, so keep your ambitions in check: the perfect is the enemy of the good.
