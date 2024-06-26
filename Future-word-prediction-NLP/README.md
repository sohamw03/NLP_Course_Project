# Intro to Natural Language Processing

# Installation 
```bash
pip3 install -r requirements.txt
python3 -m nltk.downloader popular
```

## Directories:

- All the dataSet are present in the ./dataSet folder
- All the Perplexity result are present inside the folder ./results
- The Checkpoint of the model is saved in ./SavedModel
- All the Codes are present inside ./sourceCode
- The Splitted Datasets are present at ./sourceCode/split

## Tokenization

For tokenization and cleaning I used the following embeddings :

    •	Lower case
    •	Hashtag
    •	Mentions
    •	Num
    •	Currency
    •	Url
    •	Percentage
    •	Punctuations
    •	Removing extra spaces
    •	Removal of ‘/n’

These Embeddings are clearly shown in the code with the help of comments

## Input Format:

- `python3 neural_language_model.py /workspaces/NLP_Course_Project/Future-word-prediction-NLP/SavedModel/FirstSave2.pth`

- language_model.py
  `$ python3 language_model.py <smoothing type> <path to corpus>`
  Eg=> `$ python3 language_model.py k ./corpus.txt`

- neural_language_model.py
  `$ python3 neural_language_model.py <SavedModelPath>`
  `Eg=> $ python3 neural_language_model.py ../models/trained_nlm.pth`

Then a Prompt will come whcih will ask for a sentence as input.
After entering it, it will print the preplexity of that sentence.

### NOTE: neural_language_model.py accepts sentence of length less than 34 only.

## SavedModel

- FirstSave.pth = for the corpus Pride-and-Prejudice-Jane-Austen
- FirstSave2.pth = for the corpus Ulysses-James-Joyce
