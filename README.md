# Text-to-Video-Synthesis-with-Telegram

Project title: Text to Video Synthesis with Telegram

Project Objective:  To use pre-trained LLM and vision models to present the user with the ability to generate videos based on user input text with a telegram bot interface.

### Model description
The model is text to video generation diffusion model where the input is a description text that outputs a video that matches the text description. Only English input is supported. This model has three sub-networks i.e., text feature extraction, text feature-to-video latent space diffusion model, and video latent space to video visual space with about 1.7 billion parameters.

### Telegram Bot creation
The bot is designed to generate videos based on the input text provided by users. When users send a message to the bot, it processes the text using a text-to-video synthesis pipeline from the modelscope library and sends back the generated video as a response. The bot responds to the '/start' and '/hello' commands with a welcome message and handles all other messages by generating videos based on the input text and sending them back to the users.

**Description about the files uploaded**

1. The Python script file.
2. The .mp4 files starting with text are the video results obtained from the huggingFace model.
3. The rest two .mp4 files are shows the user interaction with telegram bot.

**Running instructions**

1. Change the run time hardware accelerator to T4 GPU, if using Google Colab.
2. Run the text_to_video_synthesis_with_telegram script on Colab
3. Make sure that the script must be running while user is interacting with bot

**Interacting with telegram bot**

1. Search for text_2_video_bot username on telegram
2. User can interact with the bot
3. Bot will only respond if the script, text_to_video_synthesis_with_telegram.py, is running on Colab continuosly

As long as the script is running, telegram bot will keep polling the Telegram server for incoming messages and respond accordingly. This allows the bot to be interactive and respond to user input texts while the script is running on Colab. The script must be running continuously for the bot to be responsive to user input.

### Telegram bot interface results:

1. Video showing the user interaction
 
https://github.com/deepceptai/Text-to-Video-Synthesis-with-Telegram/assets/96874023/befe0f93-a974-46db-9352-6709eac9b84b

2. Image showing the telegram bot interface

 ![Screenshot 2023-11-25 235754](https://github.com/deepceptai/Text-to-Video-Synthesis-with-Telegram/assets/96874023/5a0e1b77-83cc-4554-9ec8-48aa9e09b6e4)

**References**

ModelScope Text to Video Synthesis: [HuggingFace](https://huggingface.co/spaces/damo-vilab/modelscope-text-to-video-synthesis)
Creating telegram bot: https://www.freecodecamp.org/news/how-to-create-a-telegram-bot-using-python/
Creating telegram bot using HuggingFace Inference API: https://cobusgreyling.medium.com/create-a-telegram-qna-chatbot-using-huggingface-inference-api-324049336557

