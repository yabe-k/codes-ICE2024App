Dataset and codes used for paper "Breaking barriers in academic communication: Insights from a novel face-to-face interaction tracking app at an international conference" (Yabe et al., in prep)

# Files

## presentations_raw.csv (not publicly available)
A list of presentations, including their titles and abstracts. This file is confidential and cannot be made public.

## presentation_doc2vec.ipynb
A Google Colab notebook containing the code used to transform presentation abstracts into vectors with Doc2Vec. The code was executed on Google Colab on 2024-11-11.
* Input: presentations_raw.csv
* Output: presentations_vectors.csv

## presentations_vectors.csv
A list of presentations represented by 50-dimensional vectors derived from the abstracts. Presentation titles and abstracts are masked.

## author_relations.csv
A table of relationships connecting attendees to presentations. These relationships include user-defined connections and those preloaded from registration data.

## attendees.csv
A list of attendees, including their research fields, countries, and registration types.

## connections.csv
A log of profile exchanges made through the app.

## analysis_and_visualization.ipynb
A Google Colab notebook containing code for data aggregation, statistical analysis, and visualization.
* Inputs: presentations_vectors.csv, author_relations.csv, attendees.csv, connections.csv
* Outputs: country_relations.gexf, field_relations.gexf, and other figures (PDF, SVG)
