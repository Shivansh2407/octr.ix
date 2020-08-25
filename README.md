# octr.ix
A Django and GraphQL based URL shortener 

Test Link - https://octrixshortener.herokuapp.com/

### Enter URL and Create Hash
![URLHash](https://github.com/Shivansh2407/octr.ix/blob/master/URLshortened.PNG)

### Error Handling
![DuplicateLink](https://github.com/Shivansh2407/octr.ix/blob/master/Error%20Handling.PNG)

```python
validate = URLValidator()
    try:
        validate(self.full_url)
    except ValidationError as e:
        raise GraphQLError('invalid url')
 ```
 
### Access the Database
![AccessData](https://github.com/Shivansh2407/octr.ix/blob/master/AccessData.PNG)

### Setup:
1. Clone the repository - `git clone https://github.com/Shivansh2407/octr.ix.git`
2. Install the requirements - `pip install -r requirements.txt (Python 2)` or `pip3 install -r requirements.txt (Python 3)`
3. Run the Server - `python manage.py runserver`
4. Go to /graphql endpoint to create the Hash - 127.0.0.1:8000/graphql
5. Access the Hashed Link by adding the Hash at the end like - 127.0.0.1:8000/{Hash}
