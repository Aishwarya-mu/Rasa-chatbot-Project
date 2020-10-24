# Rasa-chatbot-Project
A FAQ chatbot using RASA framework. This chatbot helps to answer user queries regarding the coronavirus.
# What is a chatbot?
A chatbot is an application that can initiate and continue a conversation using auditory and/or textual methods as a human would do. A chatbot can be either a simple rule-based engine or an intelligent application leveraging Natural Language Understanding. Many organizations today have started using chatbots extensively. Chatbots are becoming famous as they are available 24*7, provide a consistent customer experience, can handle several customers at a time, are cost-effective and hence, results in a better overall customer experience.
# Uses
•	Customer support

•	Frequently Asked Questions

•	Addressing Grievances

•	Appointment Booking

•	Automation of routine tasks

•	Address a query

# Prerequisites
The prerequisites for developing and understanding a chatbot using Microsoft Azure are:

•	Python installed

•	Microsoft Build tools with visual c++ 14.0 installed. Link: https://visualstudio.microsoft.com/downloads/

# Introduction to RASA
Rasa is an open source machine learning framework for building contextual AI assistants and chatbots.
Rasa has two main modules:

•	NLU for understanding user messages 

•	Core for holding conversations and deciding what to do next 

# The problem statement
The goal here is to build a chatbot which can answer queries related to the COVID-19 disease.
Technical stack:

o	Python

o	Rasa X

# Telegram Integration:
◦	Download ngrok from https://ngrok.com/download
◦	After extracting the zip file, open the ngrok file and run it.
◦	In ngrok, enter the command ‘ngrok http 5005’

•	Then go to telegram and create your own bot using Botfather:
a)	Open the telegram app and search for botfather(it is an inbuilt bot used to create other bots)
b)	Start a conversation with botfather and enter /newbot to create a newbot.
c)	Give a name to your bot
d)	Give a username to your bot, which must end in _bot.This generates an access token.

•	Open ‘credentials.yml’ and enter:
telegram:
access_token: "obtained from telegram"
verify: "your bot username"
webhook_url: "https://<ngrokurl>/webhooks/telegram/webhook"

•	Go to terminal and enter the command ‘rasa run’
•	Open one more terminal and run the command ‘rasa run actions’
•	Now, you can chat with your bot from Telegram.

# You can find the bot we created on Telegram as "covid_rasa_bot".

References:
1.	Rasa Official documentation https://rasa.com/docs/rasa/user-guide/installation/
2.	CDC Corona FAQ. 


 
