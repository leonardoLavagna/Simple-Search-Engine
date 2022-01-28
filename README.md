# Simple Search Engine(s): What is the best anime in the world?
![68747470733a2f2f696c6f766576672e69742f77702d636f6e74656e742f75706c6f6164732f323032302f30352f616e696d652d652d6d616e67612d67656e6572692e6a7067](https://user-images.githubusercontent.com/91341004/151556905-81fbfe53-f928-47ad-a54e-dbed19ffec65.jpg)

**Our goal**: Build some (simple) Search Engines over the "Top Anime Series" from the list of MyAnimeList https://myanimelist.net, using Python.

## Contributors
- Simone Chieppa
- Onur Ergun
- Leonardo Lavagna
- Leonardo Skerl
## The files below where used to test the code and to exchange data between group members (see the files branch of this repository)
- `html_pages`: folder with all the crawled anime pages
- `tsv_files.zip`: zipped folder that contains a table for each anime contained in the html_pages subfolders
- `links.txt`: contains the urls of the animes
- `vocabulary.json`: contains the vocabulary of the (parsed) words in all the animes' descriptions.
- `inverted.json`: contains the inverted index for the Search Engine 2.1
- `tfidf.json`: contains the inverted index for the Search Engine 2.2

We recommend to download the final notebook with the files and execute the appropriate cells in the notebook to check the results and carry out more queries and tests. Some markdown cells, expecially those with LaTeX formulas, can be difficult to read in the preview available here.
## Outline of the project
1. Data collection: we will save each anime page in the list in html format (see the files branch of this repository, in particular the `html_pages` folder)
2. Data parsing: we will extract (web scraping) useful informations from each anime page (e.g. Anime Title, Anime Type, Anime Popularity,...) and store them in a tsv file for each page (see the files btanch of this repository, in particular the `tsv_files.zip` folder)
3. Conjunctive query and ranking score: we will create a simple search engine (using the inverted index technique, see the files branch of this repository, in particular the `inverted.json` file) that allow the user to carry out conjunctive queries, where the queried documents will be ranked according to the `tfidf` score (see the files branch of this repository, in particular the `tfidf.json` file)
4. New Score: we will define a new custom score (instead of the tfidf score) to see how the behaviour of the search engine previously described changes
