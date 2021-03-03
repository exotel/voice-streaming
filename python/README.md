# Exotel's Streaming Demo

## Getting Started
### Overview
The demonstration script acts as a Websocket Server that conforms to Exotel's Websocket Streaming Protocol. 

### Prerequisites
```
Python 3.7 and above
```

### Installation
1. Activate virtualenv or setup a new virtualenv using [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) or [virtualenv](https://virtualenv.pypa.io/en/latest/installation.html)
2. Run
    ```
    pip install -r requirements.txt
    ```
3. The script for Unidirectional Demo uses Google Speech-to-Text API; so please enable Speech-to-Text API in Google Cloud Console. 
4. Setup and export your google credentials to your system path [Linux or MacOS](https://cloud.google.com/speech-to-text/docs/libraries#linux-or-macos), [Windows](https://cloud.google.com/speech-to-text/docs/libraries#windows)

## Run
```
python app.py --port <PORT_NUMBER> --stream_type <STREAM_TYPE>
```

## Help
```
python app.py -h
usage: app.py [-h] [--port PORT] --stream_type {unidirectional,bidirectional}

ExoWS client to enable WS communication

optional arguments:
  -h, --help            show this help message and exit
  --port PORT           Specify the port on which WS server should be
                        listening
  --stream_type {unidirectional,bidirectional}
                        Specify the type of stream
```



