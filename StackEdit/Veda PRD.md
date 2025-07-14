This is the PRD for my personal knowledge base. It will contain a function of importing and browsing.

# Importing
This will be a function that can import reading notes I've jotted down over the years. 

 - It needs to be 'smart' because these notes will not be uniform in format. I've used different apps to export my notes over the years in different formats, but this function needs to be able to parse them all the same and convert them into documents adopting a same, consistent standard format, correcting any format issues in the past while maintaining the integrity of the quotes/annotations.
 - In order for it to be 'smart', it may be necessary to include AI APIs (like Deepseek?) We cannot rely on 正则表达式 for different kinds of quote files, which will almost guarantee messed up results.
 - Regarding the format of these standardised notes, I'm thinking using either .md or .json.
 - In any event, any annotation should be attributed to a note, and any quote should be attributed to an author (or more than one authors) and a book.
 - Every time a document is imported, a list of quotes should be previewed before they are officially added to the database, so I know what are the results of parsing before they are added and we don't include messed up quotes. 
	 - At this preview stage, the user also gets to manually edit every quote/annotation as they see fit. 
	 - At this preview stage, the app will also detect any incompleteness, not lease with the punctuations. E.g. where a quote ends with a " ” " but does not start with a " “ ", it will suggest the addition of the latter at the beginning. Another example will be a missing "。" at the end of the sentence. These may be due to problems when highlighting the quotes. The suggestions are automatically incorporated but highlighted so the user knows that what were added, to ensure the overarching principle that no quote is tampered with without the user's knowledge and consent.
 - Also at this stage, an automatic de-duplication is done, so if any quote is 90% the same as an existing one, it will be highlighted and auto-deselected for import.
 - We will consider adding a function to obtain details of a book from book.douban.com by one click. But this is low priority.
 - For every book, there should be an auto-generated button to access the page for this book on book.douban.com - to achieve this function the app will search for the book (by the title and verify by name of author and any other information present) on book.douban.com and add a field containing the link in the format of, e.g. "https://book.douban.com/subject/37358287/", and the link displayed will be just "37358287" and may be manually edited.
 

# Browsing
## Search
## Reading
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQ4NDgyMDMwMF19
-->