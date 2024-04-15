# Chatbot Deployment

In this tutorial we deploy the chatbot I created in [this]([https://github.com/python-engineer/pytorch-chatbo](https://github.com/AbhayAnilark/GFG-chat-bot/tree/main/chatbot-deployment-main)t) tutorial with Flask and JavaScript.

Integrated Flask App: I've created a Flask application with Jinja2 templates to seamlessly incorporate my chatbot. Users can interact with it directly within the app.
Flask Prediction API: Alternatively, I've set up a Flask prediction API. This allows the chatbot functionality to be separated from the frontend. The HTML and JavaScript files can easily be integrated into any frontend application with minimal adjustments.


## Initial Setup:
This repo currently contains the starter files.

Clone repo and create a virtual environment
```
$ git clone https://github.com/python-engineer/chatbot-deployment.git
$ cd chatbot-deployment
$ python3 -m venv venv
$ . venv/bin/activate
```
Install dependencies
```
$ (venv) pip install Flask torch torchvision nltk
```
Install nltk package
```
$ (venv) python
>>> import nltk
>>> nltk.download('punkt')
```

Run
```
$ (venv) python train.py
```
This will dump data.pth file. And then run
the following command to test it in the console.
```
$ (venv) python chat.py
```
