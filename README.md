# word_clustering
Clustering Similar Words
Problem Statement : Case Investigators would write down summary of their investigation in the case notes field. The case notes field is free text field and can create any 
character. The idea is to form clusters on the case notes and further investigate the clusters to avoid more transmission 
They key words in this case are known and hence would be considered as supervised learning 

Data Flow
1. Read the case notes every day, combine all the case notes field to create free text field
2. Read the Case Investigator's Name, to return the clustered data along with the name
3. From the list of Keywords, use oxford dictionary API to get synonyms for them and store them on a list
4. Use Brute force search technique to compare Free Text list with Key words( along with synonyms list)
5. Return the text field containing the keyword or its synonyms while flagging them with cluster
5. Write back the data to Database 
6. Repeat Step 1 the next day

