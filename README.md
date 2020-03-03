# NetworkAnalysisCW1
Prior to running my code it is necessary to download the Bookworm Project. You can do so here: https://github.com/harrisonpim/bookworm

Prior to using Bookworm it is necessary to update some pieces of the code to run on the latest version of NetworkX. All that should be needed is to replace all instances of nx.from_pandas_dataframe with nx.from_pandas_edgelist.

'Read in Book, Create Interactions.ipynb' loads in the txt file and uses Bookworm to tokenize the text and split it into sequences. Read in the character list, and use Bookworm to calculate cooccurrence matrix and the interaction dataframe that is then used to build the networks. It also calculates different network measures to asses the size and complexity of the network.

'Plot Communities.ipynb' partitions the network nodes into communities and visualizes the network

'Centrality Measures.ipynb' uses the previously created interaction dataframe and the resulting network to calculate different centrality measures to assess which character is the main character of the story. Not all centrality measures in the notebook were used in the final analysis.

All raw data is included. All text files are book files - A Song of Ice and Fire volume 1, 2, 3, 4/5 (the final two volumes are put together as they happen simultaneously) and the complete saga (ASOIAF_FULL_NO_PARAGRAPHS.txt). ASOIAF_All_Characters.csv is the list of all character names in the entire saga. ASOIAF001_Character_Interaction_From_Excel_List.csv and similar are csv files of the interaction dataframe created and saved in the 'Read in book, create interactions.ipynb' notebook. They are then loaded into the 'Plot Communities.ipynb' and 'Centrality Measures.ipynb' notebooks.
