# AI-ASSISTANT

Virtual-AI-assistant
This virtual assistant can hear, think and respond to you. You can ask general queries (in English) about various flights. The virtual assitant will respond appropriately using its knowledge (the database). It also generates the face emoji based animation with voice as an output. It consists of speech recognition (speech to text), closed domain chatbot, speech generation (text to speech) and video rendering.

The closed domain chatbot is currently trained on the atis_flight dataset and hence it can only answer certain queries related to flights (see Queries section).

Follow How to run section to see this virtual assistant in action. It is super easy to run. The code is fully tested and works perfectly in google colab.

Main Libraries
PyTorch
SpeechRecognition
OpenCV
Sqlite3
Queries
This virtual assistant was made to help passengers book flights. It has it's own database that has Indian cities, flights and other related details. We use sqlite database maintained in a .db file (here). Following are some of the entities that are already present in the database. You can use these entities in your queries.

Database -
Cities : Pune, Mumbai, Nagpur, Chennai
Flight IDs: 1, 2, 3, 4, 5, 6, 9, 10, 11
Flight companies: Air India, Go Air, King Fisher, Indigo
Classes: Business, Economy

We will release the full structure of database soon. And, to test the bot you can ask it the following queries -

Type 1 - Hello show me flights from <city> to <city>.

Type 2 - Can you give me minimum fare for flights from <city> to <city> in the <class> class

Type 3 - Hi can you give me <flight company> flights from <city> to <city>

Type 4 - Show me details for flight with id <flight id>

Type 5 - Hey how many seats are available for flights from <city> to <city>

Currently the bot is trained only on these 5 types of queries and its all possible variations. Use natural language freely to modify your queries. The virtual assistant will help you as long as your intent is within these 5 types.

How to run
Just run the 'Virtual_assistant_notebook.ipynb' notebook in the main folder of this repository in Colab. All dependencies, models and related code is in the notebook itself.

Start executing all the cells one by one.

When you execute the last cell, it will automatically start recording your voice. When this happens you will see a button that says 'Recording' and you have to say your query at this point.

After you are done saying your query, you need to click the button to stop the recording.

The bot will show the results of your query and generate an animated face video with it's voice.
