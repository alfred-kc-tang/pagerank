# PageRank Alogrithm

The PageRank algorithm was first proposed by Larry Page, one of the founders of Google, to rank web pages in the search engine results, where more “important” web pages are ranked higher.  According to Google: it works by counting the number and quality of links to a page to determine a rough estimate of how important the website is. The underlying assumption is that more important websites are likely to receive more links from other websites. The algorithm outputs a probability distribution over all web pages, representing the likelihood that a person randomly surfing the web (randomly clicking on links) would arrive at those pages. For details, please refer to the [wikipedia page](https://en.wikipedia.org/wiki/PageRank).

Mathematically speaking, the PageRank values are the entries in the dominant eigenvector of the modified adjacency matrix in which each column’s values adds up to 1 (i.e., “column normalized”), and this eigenvector can be calculated by the power iteration method, which iterate through the graph’s edges multiple times to updating the nodes’ probabilities (‘scores’ in pagerank.py) in each iteration.

This project is only a simplified version of the PageRank algorithm.

## Table of Contents

* [Data Source](#datasource)
* [Keywords](#keywords)
* [Coding Style](#coding-style)
* [License](#license)

## Data Source

The data set is the Wikipedia adminship election data, which has almost 7K nodes and 100K edges. You may find the data on the [this page](http://networkrepository.com/soc-wiki-elec.php).

## Keywords

PageRank (PR)

## Coding Style

This project adopts the recommended practice of [PEP 8](https://www.python.org/dev/peps/pep-0008/) as well as [PEP 257](https://www.python.org/dev/peps/pep-0257/), and also by reference to [Google's Python Style Guide](https://google.github.io/styleguide/pyguide.html).

## License

This repository is covered under the [MIT License](https://github.com/alfred-kctang/pagerank/blob/master/LICENSE).
