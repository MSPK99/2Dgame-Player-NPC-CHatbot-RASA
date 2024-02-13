
# Project Name : RASA CHATBOT -> Player <=> NPC  Conversations

A dynamic chatbot integration for 2D game environments, facilitating engaging conversations between players and NPCs.

## Features

- **Dynamic NPC Conversations**: Leverages NLU (Natural Language Understanding) for NPCs to respond dynamically to player inputs.
- **Customizable Responses**: Utilizes `domain.yml` to define and expand NPC responses for unique interactions.
- **Integration with Game Mechanics**: Easily integrates with 2D game engines, enhancing player immersion.
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

- A compatible 2D game engine.
- Basic knowledge of Python and YAML.

### Installation
1. Having pycharm is recommended. Makes things easier when using rasa
2. Set up a virtual environment (optional but recommended) for Python dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```
3. Check Rasa Dependencies at the end
4. Install Rasa within the virtual environment:
   ```bash
   pip install rasa
   ```
5. Clone the repository to your local machine or game project directory.
6. Have a reasonable understanding about rasa files. if not create a demo project using 
   ```bash
   rasa init
   ```
7. simply replace these .yml or .py files in their stead and should work just fine


8. Follow the configuration instructions in `config.yml` for NLU model and dialogue management.
9. Integrate `actions.py` into your game's event handling system.

10.  Then to train ur rasa model  
   ```bash
    rasa train
   ```
11. once ur model has been trained. its recommended to create a new terminal and run
   ```bash
   rasa run actions
   ```
12. finally to converse 
   ```bash
   rasa shell
   ```

## Usage

- **Customize Intents and Responses**: Edit `domain.yml` for game-specific intents, entities, and responses.
- **Define Conversation Paths**: Use `stories.yml` for scripting conversation flows based on player choices.
- **Implement Custom Actions**: Extend `actions.py` with game-specific logic for dynamic interactions.
- **Integration with Game Engine**: Embed the chatbot in your game, processing player inputs and bot responses within the game context.
- **Testing and Iteration**: Continuously refine the chatbot based on player feedback and testing.

## Contributing

Contributions are welcome! See [CONTRIBUTING.md](link-to-code-of-conduct) for guidelines.

## Contact

For inquiries or proposals, contact me at praneethkumar.m@yahoo.com.


## Dependencies:  ( check the versions for further compatability errors)

absl-py==1.4.0
aio-pika==8.2.3
aiofiles==23.2.1
aiogram==2.25.2
aiohttp==3.8.6
aiohttp-retry==2.8.3
aiormq==6.4.2
aiosignal==1.3.1
APScheduler==3.9.1.post1
astunparse==1.6.3
async-timeout==4.0.3
attrs==22.1.0
Babel==2.9.1
bidict==0.22.1
boto3==1.34.35
botocore==1.34.35
CacheControl==0.12.14
cachetools==5.3.2
certifi==2024.2.2
cffi==1.16.0
charset-normalizer==3.3.2
click==8.1.7
cloudpickle==2.2.1
colorama==0.4.6
colorclass==2.2.2
coloredlogs==15.0.1
colorhash==1.2.1
confluent-kafka==2.3.0
cryptography==42.0.2
cycler==0.12.1
dask==2022.10.2
dnspython==2.3.0
docopt==0.6.2
fbmessenger==6.0.0
fire==0.5.0
flatbuffers==23.5.26
fonttools==4.47.2
frozenlist==1.4.1
fsspec==2024.2.0
future==0.18.3
gast==0.4.0
google-auth==2.27.0
google-auth-oauthlib==1.0.0
google-pasta==0.2.0
greenlet==3.0.3
grpcio==1.60.1
h11==0.14.0
h5py==3.10.0
httptools==0.6.1
humanfriendly==10.0
idna==3.6
jax==0.4.23
jmespath==1.0.1
joblib==1.2.0
jsonpickle==3.0.2
jsonschema==4.17.3
keras==2.12.0
kiwisolver==1.4.5
libclang==16.0.6
locket==1.0.0
magic-filter==1.0.12
Markdown==3.5.2
MarkupSafe==2.1.5
matplotlib==3.5.3
mattermostwrapper==2.2
ml-dtypes==0.3.2
msgpack==1.0.7
multidict==5.2.0
networkx==2.6.3
numpy==1.23.5
oauthlib==3.2.2
opt-einsum==3.3.0
packaging==20.9
pamqp==3.2.1
partd==1.4.1
pillow==10.2.0
pluggy==1.4.0
portalocker==2.8.2
prompt-toolkit==3.0.28
protobuf==4.23.3
psycopg2-binary==2.9.9
pyasn1==0.5.1
pyasn1-modules==0.3.0
pycparser==2.21
pydantic==1.10.9
pydot==1.4.2
PyJWT==2.8.0
pykwalify==1.8.0
pymongo==4.3.3
pyparsing==3.1.1
pyreadline3==3.4.1
pyrsistent==0.20.0
python-crfsuite==0.9.10
python-dateutil==2.8.2
python-engineio==4.9.0
python-socketio==5.11.1
pytz==2022.7.1
pywin32==306
PyYAML==6.0.1
questionary==1.10.0
randomname==0.1.5
rasa==3.6.16
rasa-sdk==3.6.2
redis==4.6.0
regex==2022.10.31
requests==2.31.0
requests-oauthlib==1.3.1
requests-toolbelt==1.0.0
rocketchat-API==1.30.0
rsa==4.9
ruamel.yaml==0.17.21
ruamel.yaml.clib==0.2.8
s3transfer==0.10.0
sanic==21.12.2
Sanic-Cors==2.0.1
sanic-jwt==1.8.0
sanic-routing==0.7.2
scikit-learn==1.1.3
scipy==1.12.0
sentry-sdk==1.14.0
simple-websocket==1.0.0
six==1.16.0
sklearn-crfsuite==0.3.6
slack_sdk==3.26.2
SQLAlchemy==1.4.51
structlog==23.3.0
structlog-sentry==2.0.3
tabulate==0.9.0
tarsafe==0.0.4
tensorboard==2.12.3
tensorboard-data-server==0.7.2
tensorflow==2.12.0
tensorflow-estimator==2.12.0
tensorflow-hub==0.13.0
tensorflow-intel==2.12.0
tensorflow-io-gcs-filesystem==0.31.0
termcolor==2.4.0
terminaltables==3.1.10
threadpoolctl==3.2.0
toolz==0.12.1
tqdm==4.66.1
twilio==8.2.2
typing-utils==0.1.0
typing_extensions==4.9.0
tzdata==2023.4
tzlocal==5.2
ujson==5.9.0
urllib3==2.0.7
wcwidth==0.2.13
webexteamssdk==1.6.1
websockets==10.4
Werkzeug==3.0.1
wrapt==1.14.1
wsproto==1.2.0
yarl==1.9.4