Wikipedia Search Engine

For indexing:
	run parcerc.java with 2 arguements - wikidump and indexfilename
	multiple index files are created in chunks of 5000 pages
	run merge.java to merge to multiple index files into 36 files(0-9a-z)
	run secondindex.java to create 36 secondary index files 
	run secondary.java and tertiary.java to create index of title file

for running queries:
	run query.java
	for free text query just enter the text. top 10 relevant documents are retrieved based on tf-idf score
	example - "sachin tendulkar"  (without the quotes)
	for field query:-
			t:title
			b:body
			c:category
			i:infobox
			l:external links
			r:references
	example - "t:sachin b:ecommerc"
				 
