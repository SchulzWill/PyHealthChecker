# PyHealthChecker

PyChecker is a Python 3.7 RESTful health-checker API using Flask, SQLite, and APScheduler. 

## Installation on Dev Environment

Clone this repository and then run use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.

```bash
pip install -r ./requirements.txt
```
After packages installation , run ./app.py
```bash
python3 run app.py
```

## Running in Docker

Clone this repository and then run:
```bash
docker build . -t pyhealthchecker
```

Once the image has been built, run
```bash
docker run -p 5000:5000 pyhealthchecker
```

## Testing
There is a [Postman Collection](https://www.getpostman.com/collections/6e3e8503d5700333b99f) available for local and remote tests

You can also run the ./load.sh to make some initial requests and validations.

On Linux and MacOS environments, you will need to give permissions to the bash file:
```bash
chmod +x load.sh 
```
Now, run the curl initial file
```bash
./load.sh
```

All logs will be written on ./app.log .

## Distributing
The docker image of this project is available at [Docker Hub](https://hub.docker.com/r/schulzwill/pyhealthchecker) and can be pulled and executed independently:
```bash
 docker pull schulzwill/pyhealthchecker
```


## Contributing
Pull requests are welcome. 
For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)