# Django
1. Create Virtual Env: py -m venv ujayreact
2. Activate the Env: ujayreact\Scripts\activate.bat
3. Install all requirements: pip install -r req.txt
4. Create a Django Project  : django-admin startproject bckend
5. get into django project: cd bckend
6. create app: python manage.py startapp api
7. move req.txt back into bckend folder
8. create a serializer.py file
9. Meta Class: Defines the model and fields to include in the serialization process.
   9.1.A. extra_kwargs: Additional settings for specific fields. Here, it ensures that the password is write-only (not returned in API responses).
   9.1.B. extra_kwargs to be written in dictionary format
10. **validated_data unpacks the dictionary into keyword arguments, effectively calling:
    10.a. Validated data: {
                          'username': 'ujayreat',
                          'password': 'password12',
                          'email': 'ujayreat@example.com'
                          }

    10.a. User.objects.create_user(username='ujayreat', password='password12', email='ujayreat@example.com')
11. Self is the first parameter of any method in a class, and it allows us to access the instance's attributes and other methods from within the class.
12. Axios is a popular HTTP client for making requests to servers. You can use it to fetch data from APIs, send data to servers, etc.
