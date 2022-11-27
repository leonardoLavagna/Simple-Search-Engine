# Simple Search Engine(s): What is the best anime in the world?
![68747470733a2f2f696c6f766576672e69742f77702d636f6e74656e742f75706c6f6164732f323032302f30352f616e696d652d652d6d616e67612d67656e6572692e6a7067](https://user-images.githubusercontent.com/91341004/151556905-81fbfe53-f928-47ad-a54e-dbed19ffec65.jpg)

Our goal is to  build some (simple) Search Engines over the "Top Anime Series" from the list of MyAnimeList https://myanimelist.net, using Python. We followed these steps:
  1. **Data collection**: each anime page is saved in a list in html format (see the files branch of this repository, in particular the `html_pages` folder)
  2. **Data parsing**: by web scraping useful informations from each anime page has been extracted (e.g. Anime Title, Anime Type, Anime Popularity,...) and  stored in a tsv file for each page (see the files btanch of this repository, in particular the `tsv_files.zip` folder)
  3. **Conjunctive query and ranking score**: a simple search engine (using the inverted index technique, see the files branch of this repository, in particular the `inverted.json` file) is created that allow the user to carry out conjunctive queries, where the queried documents will be ranked according to the `tfidf` score (see the files branch of this repository, in particular the `tfidf.json` file)
  4. New Score: a new custom score (instead of the tfidf score) is defined to see how the behaviour of the search engine previously described changes

### What's in here?
There are two branches: `main` and `files`. In the branch `files` the following files where used to test the code and to exchange data between group members )
- `html_pages`: folder with all the crawled anime pages
- `tsv_files.zip`: zipped folder that contains a table for each anime contained in the html_pages subfolders
- `links.txt`: contains the urls of the animes
- `vocabulary.json`: contains the vocabulary of the (parsed) words in all the animes' descriptions.
- `inverted.json`: contains the inverted index for the Search Engine 2.1
- `tfidf.json`: contains the inverted index for the Search Engine 2.2
In the `main` branche there is the notebook with all the code and comments of the project `main.ipynb` 

We recommend to download the final notebook with the files and execute the appropriate cells in the notebook to check the results and carry out more queries and tests. Some markdown cells, expecially those with LaTeX formulas, can be difficult to read in the preview available here.

### Dataset
The dataset was created by us by web scraping the page https://myanimelist.net/topanime.php.

### Disclamair
This project was part of a course of Algorithmic Methods of Data Mining at Sapienza University of Rome held by Prof. Aris Anagnostopoulos. This project was done in collaboration with Simone Chieppa, Onur Ergun, and Leonardo Skerl

