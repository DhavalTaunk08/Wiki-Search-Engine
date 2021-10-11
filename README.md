# Wiki-Search-Engine

I did this project in the course **Information Retrieval and Extraction** during my **MS by Research @ IIITH**. This project contains code for creating a search engine from scratch in python.

Libraries used are **NLTK, PyStemmer, xml.Sax, re, math etc**.

The search engine is implemented in 2 languages viz english and hindi.

Link to the data is given below:-

[English dump](https://dumps.wikimedia.org/enwiki/20210720/enwiki-20210720-pages-articles-multistream.xml.bz2)
[Hindi dump](https://dumps.wikimedia.org/hiwiki/20210720/hiwiki-20210720-pages-articles-multistream.xml.bz2)

If you want to create index for english language, you can try below command:-
 ```
 python3 english_indexer.py path_to_xml_dump
 ```

And for hindi you can try:-
 ```
 python3 hindi_indexer.py path_to_xml_dump
 ```
 
To run the search for english, you can try below command
```
python3 english_search.py --filename queries.txt --num_results 15
```

The fields **--filename** and **--num_results** are optional. By default **--num_results** is initilaized to **10**. And if you don't pass **--filename** parameter, it will prompt you to enter query on command line.

For hindi, you can try below command.

```
python3 hindi_search.py --filename queries.txt --num_results 15
```
The queries file should contain queries on seperate lines.
