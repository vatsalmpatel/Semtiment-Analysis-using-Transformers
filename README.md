# Sentiment Analysis using the Hugging Face 🤗 Transformers

In this example, we are gonna look at the BERT Transformer model from Hugging Face that will be used fro Sentiment Analysis. 

The BERT Model is trained on product reviews from six languages:

- English
- Dutch
- German
- French
- Spanish
- Italian

We can leverage this trained model and use it very easily to get sentiments from reviews, I mean any reviews 🍾 from any of those 6 languages 💬.

# How to run the notebook, you might ask ❓

To that I would say, a very good question. In order to run the notebook, you need to install some dependencies first, and enable some `developer' features within `Windows`, in order to load the model from Hugging Face 🤗.

First, lets install some dependencies. In order to do so, you need to create an environment using Anaconda or any other environment manager you perfer (I prefer Anaconda) and do the following:

```Bash
conda create -n new_env_name
```

After you have created the encironment, activate it using

```Bash
conda activavte new_env_name
```

After this you need to install all the dependencies from the `requirements.txt` file:

```Bash
pip install -r requirements.txt
```

Once this is done, you also need to enable developer inside windows, to do that you need to search `Developer` in Windows Search and then go to `Developer Settings`. Enable the option and restart your computer. Once this is enabled, if you are using `Jupyter Notebook` you need to open the command prompt as `Administrator` and then run Jupyter Notebook.

# Introduction to the Notebook 📓

The notebook has a total of 5 sub-parts, that we will use to load the model from Hugging Face 🤗 and use to perform sentiment analysis.

▶ `Imports` provides all the necessary imports that will be needed to perform sentiment analysis.

▶ `Instantiating and setting-up the model` initializes the tokenizer from the model to tokenize all the sentences using the model from the Hugging Face 🤗 website.

Link to the model used in the example: https://huggingface.co/nlptown/bert-base-multilingual-uncased-sentiment

▶ `Encode and Calculate the Sentiment` will use the tokens generated from the model and use the model to perform sentiment analysis. As you will see, this is very easy using the Huggin Face Transformers.

▶ `Collect reviews from the web` is a small script that will go on yelp and scrape reviews from a specific restaurant's page and store them.

▶ `Load Reviews into Dataframe`, will load all the collected reviews into a DataFrame and perform sentiment analysis on all the reviews and append sentiment score as a new column in a DataFrame.

# How to interpret the sentiment scores ❓

Well, it is quiet simple, `1` represents the worst possible review and a score of `5` is the best possible review.

---

### ✅🏁
### And that was it, you just performed sentiment analysis using the Hugging Face 🤗 transformer model, and that too with ease. You can leverage these models for rating movie reviews and much more.