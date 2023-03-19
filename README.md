# Sample code to compleat Immersive lab's **Dependency Confusion** lab.

Please note that ```client.py``` and ```server.py``` reverse shell implementation I took from free chapter of the [Ethical Hacking with Python](https://www.thepythoncode.com/article/create-reverse-shell-python) book.

### Create new package by modifying existing one.
Download any package from mocked PyPi server, unpack, replace  ```setup.py``` with content of ```client.py```, rename folder and increment  dependency version. Archive it back and upload to server.

### Upload to server
twine upload --repository-url http://<ip of mocked server> dist/*


PS. You can run ```client.py``` and ```server.py``` locally to get an idea. By default `client.py` mapped to localhost.