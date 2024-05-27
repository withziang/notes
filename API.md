# Note on Making an API using Python

## Flask
Most import methods: *Flask, request, jsonify*

### API endpoint setup

```
app = Flask(__name__)
@app.route('/route', methods=['POST'])
def function():
  ...
@app.route('/route', methods=['GET'])
def function():
  ...
```

### Retrieve request data
Using *requests*, we can read data from the requester.

- Json file, in POST method
  ```
  paras = request.get_json()
  ```
- single argument, in get method
  ```
  s = request.args.get('para')
  ```

### APi running setup
```
if __name__ == "__main__":
    app.run(host='0.0.0.0')

```
OR
```
if __name__ == "__main__":
    app.run()

```


## Request
How to request an api

### Using Response.status_code
```
if response.status_code == 200:
        return response.json() 
    else:
        print(f"API failed")
        return response.json()
```
### Request a GET API
- Define url
- ```
  response = requests.get(url, params={some dictionary})
  ```

### Request a POST API
- Embed API key
  ```
  def getHeaders():
    load_dotenv()  # load .env file
    apikey = os.getenv('xxx')
    headers = {
        'Authorization': f'{apikey}'
    }
    return headers
  ```
- ```
  response = requests.post(url, headers=headers, json=postData)
  ```




