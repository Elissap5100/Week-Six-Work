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
- Once I pinpoint the various places he goes, I may be able to use this tool to highlight when exactly he goes from place to place!

## Step 4: Topic Modeling with the TMTool
- Honestly I was just overall curious to see if this would work with one massive text files, and not many. Technically, that one text files has many different entries that if organized could be turned into many different files and place in its on directory. I want to see if it still pulls topics from the text file like it is now.
-It was not working with just one, so I attmpted doing the process with the original txt file as well, but the results were seemingly unusable. I think this technique is more for large scale sets of data, not a single and sparingly filled out journal.
- In what little I did understand from analyzing the results, there were a lot of names (mainly annie and Tom) jumbled in the data that reccured alot. There was mention of "letter" as well. This leads me to believe my assumptions are based somewhat on fact that Claire really cared about her family.
- As usual, all created files will be in the repository in the folder labelled "tmt output"

## Step 5: Text Analysis with Antconc
-This last attempt to analyze the data is more of a leap in the dark to see if 
        - A: It will even work (might have the same problem as last step and'
        - B: If my findings line up with the Voyant step
- Fortunately, this tool seemingly worked much better than the last one. I used to again explore the data, or diary entries and see when certain names or topics appear in what context.

![Wordlist](https://github.com/Elissap5100/Week-Six-Work/blob/master/New%20folder/antA.PNG)

- To kick start my plan a small bit, I outputted a file of all the times "letter" was used in her diary. From there, I belive I can more eaily track Tom's movement with the military by simply "ctrl + find-ig" all the letters and ready what they say. By my estimate there is over 30 of them.

Here is instances of just the word "letter":

![Letter](https://github.com/Elissap5100/Week-Six-Work/blob/master/New%20folder/letters.PNG)

Here are the instances of letter from Tom:

![TomLetters](https://github.com/Elissap5100/Week-Six-Work/blob/master/New%20folder/FromTom.PNG)


![TomLetters](https://github.com/Elissap5100/Week-Six-Work/blob/master/New%20folder/tomlines.PNG)

- All files are in the repository in the folder called "New Folder". (An unfortunate name that I could not figure out how to change through github)

### How will I display the data I found?    
**Instructions:** You will share your results using an appropriate technique you encountered in week 5. Other possibilities are ok too; just check with Dr. Graham first. Remember, you don’t have a lot of time, so keep your ambitions in check: the perfect is the enemy of the good.

- As I have mentioned throughout the first part of this project, I wish to make a story map recounting where To moved during his deploymment in 1942. Each new spot I will include an image (if I can find a good one), the date, the text from the letter and ofcourse the location. I think It will be an interesting Narrative to come from Claire's journal.
- A major concern of mine is discovering who Tom was exactly to Claire because I seem to not know as of right now. I suspect he is her husband but I am not completely sure. I am hoping through exploration of these letters I will learn more.

**Update:** Through further investigation of the diary, I have determined that Tom is Claire Paine's brother and I belive Ruth is Tom's wife who is good friends with Claire and her sister Annie. I realize this is an assuption but there are many factors that indicate this may be correct. The following line was a good indicator of their relationship (plus no mention of anything more than platonic care for him from Claire's perspective):

```
After lunch shopped around – Annie bought a new dress, blue with white stripes – Claire a new hat, dusty rose shade made of bands of ribbon – Tom went home to sleep, he was tired – It seemed so good to have Tom with us, He’s still very fond of home and Mother.

Tom loves our home & our yard, I think sometimes he is a little homesick for his boyhood home & big lawn
```
It is now confirmed, Tom is Married to Ruth and I can only assume he is Claire's brother:
```
July 31 1942 Fri:  Tom & Ruths 3rd wedding anniversary.
```

I stand corrected, I believe Tom is her Nephew?
```
October 291942 Thur:  Another letter from Tom.  Its nice to have a fine nephew like Tom.  A fine young man – Two Capitals & the money belt were rec’d by him & he was so pleased – His work friend at Douglass Plant in California has gone into service with his son.
```

The following text I thought was cool (Go Canada!):
```
At 8:30 we listened to “Cheers from the Camp” from Camp Borden in Canada – Its sponsored thru Genl Motors by the Canadian & Amer. Governments – Its closing song was “God Bless America-“ Canada is so sincere, so determined & courageous – fine bunch of boys there.
```
**Here is my Thought Process in Creating the Story Map:**
There are many letters to and from Tom so I have decided to call this "Letters of Tom" (1942). I wish I had the ability to learn more of these two people, but due to time restraints I do not. I have just put together an organized list of sorts of all the letters to and from Tom from Claire Eva Paine's perspective in 1942. There is not too much detail in each letter but some do offer information of where he is and what he is doing at the Time. For the purpose of a story map (and the fact that I am missing pictures/videos/media to attach to some moments) I am thinking of only including the messages where he moves somewhere or something happens. If I can not find a relatable historical piece of media, I will attach the image of her journal entry to that point. 

**Here are some links I accessed when creating my Story Map and finding ressources to display:**
- https://millercenter.org/the-presidency/presidential-speeches/february-23-1942-fireside-chat-20-progress-war
- https://web.archive.org/web/20090210105312/http://nrhs.com/archives/rea.htm
- http://loc.gov/pictures/resource/cph.3c27693/
- http://docs.fdrlibrary.marist.edu:8000/BROWSE.cgi?db=2&pos=450&inc=50
- https://www.latimes.com/visuals/photography/la-me-fw-archives-southern-california-world-war-ii-aircraft-manufacturing-20180730-htmlstory.html
- https://hslb.org/product/ocean-blvd-1930/
- https://www.archives.gov/news/articles/merchant-marine-records-document-maritime-service
- https://hslb.org/wp-content/uploads/2014/01/R0056-P-5028-1930-Ocean-Blvd1.jpg
- https://www.ibiblio.org/hyperwar/USN/ref/USN-Act/VA.html
- http://www.boeing.com/companyoffices/gallery/C8AB-RedBarn.html
-https://www.history.navy.mil/our-collections/photography/wars-and-events/world-war-ii/pearl-harbor-raid/post-attack-ship-salvage/general-views/NH-64303.html
- https://1940census.archives.gov/search/?search.census_year=1940&search.city=Long%20Beach&search.county=&search.enumeration_district=59-1&search.page=1&search.range_end=59-144&search.range_start=59-1&search.related_type=map&search.result_type=map&search.state=CA#city=long-beach&county=los-angeles-county
- http://www.usmm.org/trainingship.html
- http://www.usmm.org/postertrain2a.html
- http://hamptonroadsnavalmuseum.blogspot.com/2015/08/remembering-project-much-bigger-than.html
- https://en.wikipedia.org/wiki/Valley_Forge
- https://www.unionstation.org/timeline
- https://www.chicagorailfan.com/stbckcy.html
- http://mdh.contentdm.oclc.org/cdm/landingpage/collection/kcpltax
-https://www.history.navy.mil/browse-by-topic/heritage/uniforms-and-personal-equipment/uniforms-1942-1943.html
- https://www.portofhueneme.org/about/port-history/
- https://seabeemagazine.navylive.dodlive.mil/2014/11/26/harbor-base-neighbors-when-the-navy-came-to-port-hueneme-1942-1945-and-beyond/
- http://hamptonroadsnavalmuseum.blogspot.com/search/label/Camp%20Bradford

<iframe src="https://uploads.knightlab.com/storymapjs/06af2dd60026226f1e0a9ea7326aac8d/letters-of-tom/index.html" frameborder="0" width="100%" height="800"></iframe>
