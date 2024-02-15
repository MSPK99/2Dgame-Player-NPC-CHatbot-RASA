
# RASA CHATBOT -> Player <=> NPC  Conversations

A dynamic chatbot integration for 2D game environments, facilitating engaging conversations between players and NPCs.

## Features

- **Dynamic NPC Conversations**: Leverages NLU (Natural Language Understanding) for NPCs to respond dynamically to player inputs.
- **Customizable Responses**: Utilizes `domain.yml` to define and expand NPC responses for unique interactions.
- **Integration with Game Mechanics**: working towards integrating chatbot with 2D game engines, enhancing player immersion.
- **Scalable Conversation Logic**: Employs `stories.yml` and `rules.yml` to evolve conversation flows based on player actions or progress.
- **AGPL Licensed**: Promotes community sharing and improvements.

## Why AGPL?

This project is under the GNU Affero General Public License (AGPL), ensuring modifications are available under the same license to foster transparency and collaboration.

## Getting Started

### Prerequisites

- **Python 3.6+**(Latest version recommended) installed. [Download Python](https://www.python.org/downloads/)
- **Rasa Open Source** for NLU and dialogue management. Install with pip:

  ```bash
  pip install rasa
  ```
- Basic knowledge of Python and YAML.

### Installation
1. Having pycharm is recommended. Makes things easier when using rasa
2. Set up a virtual environment (optional but recommended) for Python dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```
3. Install Rasa within the virtual environment:
   ```bash
   pip install rasa
   ```
4. Check Rasa Dependencies at the end
   ```bash
   pip install -r requirements.txt
   ```

5. Clone the repository to your local machine or game project directory.
6. Have a reasonable understanding about rasa files. if not create a demo project using 
   ```bash
   rasa init
   ```
7. simply replace these .yml or .py files in their stead and should work just fine


8. Follow the configuration instructions in `config.yml` for NLU model and dialogue management.

9. Then to train ur rasa model  
   ```bash
   rasa train
   ```
10. Once ur model has been trained. its recommended to create a new terminal and run
    ```bash
    rasa run actions
    ```
11. Finally to converse 
    ```bash
    rasa shell
    ```

## Usage

- **Customize Intents and Responses**: Edit `domain.yml` for game-specific intents, entities, and responses.
- **Define Conversation Paths**: Use `stories.yml` for scripting conversation flows based on player choices.
- **Implement Custom Actions**: Extend `actions.py` with game-specific logic for dynamic interactions.
- **Integration with Game Engine**: Embed the chatbot in your game, processing player inputs and bot responses within the game context.
- **Testing and Iteration**: Continuously refine the chatbot based on player feedback and testing.




## Sample Conversation :

Below is an example of a conversation using the chatbot in its current iteration. As the project is in the initial phase, the dialogue showcases the chatbot's current capabilities and areas where refinement and expansion are needed.

  ![Screenshot 2024-02-13 112608](https://github.com/MSPK99/2Dgame-Player-NPC-CHatbot-RASA/assets/157824384/58503eec-7be3-4b27-b3f4-d30697abe7d9)



## Room for Improvement
The chatbot is still in the early stages of development, and there are several key areas where we are focusing on improvements:

- **Contextual Understanding**: Enhancing the chatbot's ability to understand the context of the conversation and maintain coherence throughout interactions.
- **Response Variability**: Increasing the variability and complexity of responses to avoid repetition and create a more dynamic conversation.
- **Emotional Intelligence**: Improving the chatbot's capability to recognize and appropriately respond to the emotional content of user inputs.
- **Game Integration**: Further developing the integration with game mechanics to provide a seamless experience between gameplay and chatbot interactions.

I welcome contributions, especially in these areas, to help evolve the chatbot's conversational abilities and integration into the gaming environment.


## Contributing

Contributions are welcome! See CONTRIBUTING.md [(link-to-code-of-conduct)](https://github.com/MSPK99/2Dgame-Player-NPC-CHatbot-RASA/blob/main/CONTRIBUTING.md) for guidelines.

## Contact

For inquiries or proposals, contact me at praneethkumar.m@yahoo.com.

webexteamssdk==1.6.1
websockets==10.4
Werkzeug==3.0.1
wrapt==1.14.1
wsproto==1.2.0
yarl==1.9.4
