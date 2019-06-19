# ConvAI bot#


## Installing

Download and put trained models to folders:

```
./setup.sh
```

Build containers:

```
docker-compose -f docker-compose.yml -f telegram.yml build
```

Setup config.py, do not forget to put TELEGRAM token:

```
cp dialog_tracker/config.example.py dialog_tracker/config.py
```

dialog_tracker/config.py should look like this:

```
WAIT_TIME = 15
WAIT_TOO_LONG = 60
version = "17 (24.12.2017)"
telegram_token = "your telegram token"
```

## Running the bot

This command will run the telegram bot with your telegram token:

```
docker-compose -f docker-compose.yml -f telegram.yml up
```

# Running the tests

Run the bot by using json api server:

```
docker-compose -f docker-compose.yml -f json_api.yml up
```

Run the tests:

```
python dialog_tracker/tests/test_json_api.py http://0.0.0.0:5000
```


