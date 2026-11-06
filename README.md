# Movie Data Analysis

I combined five decades of Wikipedia movie data and explored how often genres and actors appear in the records.

**Python · Pandas · NumPy · Matplotlib**

[Open the notebook](Movie_Industry_Analysis.ipynb)

## Data and preparation

The notebook loads the 1960s, 1970s, 1980s, 1990s and 2000s JSON files from [wikipedia-movie-data](https://github.com/prust/wikipedia-movie-data). It keeps titles, years, cast lists and genres, removes rows with missing values, and combines the files into one table.

The saved run contains **10,750 films covering 1960–2009**. Each film can have several genres and actors, so I expand those lists before counting them.

## What I found

- Comedy and Drama have the most genre entries: **3,777** and **3,758**, followed by Action with **1,228**.
- Gene Hackman has **71** cast credits in this dataset, followed by Robert Duvall with **68** and Robert De Niro with **65**.
- The notebook plots annual counts for the three leading genres and actors, then compares the top ten actors' credits in the leading genres.

These counts describe this collection. They do not measure audience popularity or box-office success. A film can count toward more than one genre; percentages in the top-ten pie charts refer only to the displayed entries.

## Run it

Use Python 3 and install the dependencies:

```bash
pip install -r requirements.txt
jupyter notebook Movie_Industry_Analysis.ipynb
```

You can also upload the notebook to Google Colab. Run the cells from top to bottom with an internet connection; the notebook downloads the JSON files and writes `movies_data.csv` locally. The source can change, so a new run may differ from the saved outputs.

Educational project completed during GoIT Data Analytics training.
