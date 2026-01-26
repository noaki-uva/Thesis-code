# Thesis-code
From Rules to Models Machine Learning–Based Legal Reference Detection in Dutch Court Rulings
To scrape the code you use file scraper.ipynb
you need the selium chrome exe file in the same map

if this is the second time you run the scraper uncomment the load in with pickle and comment the creation of the dict in the next code block in the file.
if you want to change how many court rulings you scrape change variables , saves and max_number

after this code has been run everything will be saved in a pkl

after this run the training and test data.
this will produces 3 sets of training data, test data.
Logistic regression data, spacy data,roberta data.
you can then train the logistic regression Model in lg train.ipynb
and train any spacy model or roberta model with the other sets of data.
to get evaluation data run evaluation_data.ipynb . it scrapers unvisted sites and makes a different set of spacy format data("test",{enteties:[(1,2 , label)]} .(not a spacy file)

after this run the evaluation files of each model. called lg_eval.ipynb, spacy_eval.ipynb,robertera_eval.ipynb
