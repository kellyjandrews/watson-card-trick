# IBM Watson Card Trick

Steps to run:

1. Create [IBM Voice Agent on IBM cloud](https://cloud.ibm.com/catalog/services/voice-agent-with-watson)
1. [Buy a Nexmo number](https://dashboard.nexmo.com/buy-numbers)
    1. Add SIP forwarding
    1. Add the SIP uri from the Voice Agent
1. Create a new voice agent in your instance
    1. Add the Nexmo number
    1. This step creates all other services
1. Go to Watson Assistant and import the skill JSON
1. After creating the agent, edit the following
    1. Change the kill to use "Card Trick"
    1. Update the Speech model to US Broadband
    1. Change the voice to use DNN technology

You can then dial the number, and give it a password from the `magic-key-words.pdf` file to have Watson tell you your card. 
