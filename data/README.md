# Friends

This dataset describes a character-interaction network for the TV series _Friends_. The available file, `friends_episodes.txt`, is a plain-text collection of episode-level interactions in which nodes are characters and links represent that two characters interact during an episode. When all repeated interactions are aggregated, the resulting network is naturally interpreted as undirected and weighted, with weights counting how often a pair of characters appears together.

The scope of the text file is broader than the older “first season” description might suggest. The episode markers in `friends_episodes.txt` run from `s1e1` through `s10e18`, for a total of 269 marked episodes, so the file spans multiple seasons. In the raw text, lines beginning with `#` identify episode headers, while each non-comment line contains a pair of character names representing one observed interaction.

The dataset was manually generated and curated by Prof. Ana Bazzan. If you use this dataset, please acknowledge this repository and/or the following publication: Bazzan, Ana LC. “I will be there for you: clique, character centrality, and community detection in Friends.” _Computational and Applied Mathematics_ 39.3 (2020): 1-25. A preprint is available at <https://arxiv.org/abs/1804.04408>.

The file can be used as input for graph-processing software such as igraph, provided that the parser accounts for comment lines and episode headers. Some comment lines also contain extra notes about episode types, so a small amount of regular-expression-based cleaning may be useful when importing the data into other tools.

A note about license: THE DATASET IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE DATASET OR THE USE OR OTHER DEALINGS IN THE DATASET.
