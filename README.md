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
