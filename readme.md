## Coding Challenge

### Project Setup
* Clone from the repository
* Move to the root folder
* Create virtual environment (You can use `python3 -m venv venv`)
* Active virtual environment
* Install dependencies w/ requirements.txt (`pip install -r requirements.txt`)
* Run the project by (`python run.py`)

The development server will be Up and running

Open your postman or http client and do following:

* API Endpoint GET & POST: `http://127.0.0.1:8080/api/v1/post-data/`

### GET request response:
`
{
    "status": true
}
`

### POST request body:
```
{
    "is_malicious": false,
    "name": "Adrian Badilla",
    "position": "Python Developer"
}
```
### POST request response:
if is_malicious is true
```
{
    "error": "Data unauthorized"
}
```
status code: 401

if is_malicious is false
```
{
    "is_malicious": false,
    "name": "Adrian Badilla",
    "position": "Python Developer"
}
```
status code: 200

### Log file
When server will be runing, logger file will be created as `errors.log` with all information logged.

Te have a look on log data, open 
errors.log 
