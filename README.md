# Testreadme


**API that create an encrypted zip file**
Steps  | explanation
------------- | -------------
0  | make sure that you have python version 3.11.1 installed on your machine, if not download it from here : https://www.python.org/downloads/
1  | Put the files Api.py, keys.py, pgp_encryption.py, and requirements.txt in the same folder
2  | Open a terminal inside that folder and execute the command `pip install -r requirements.txt`
3  | Inside the folder run `python .\api.py` (if it doesnt work, run `python3 .\api.py`)
4.0  | Once the application is running, put a **POST** request of the following link http://127.0.0.1:5000/create_secure_ptr in postman and give it 2 arguments in the body the `ptr_number`(8 digits of the ptr number) and `file`(One or more file to be zipped)
4.1	| A curl example is : `curl -v -F ptr_number=12345678 -F file=@C:\Users\houledamarbencheikh\Desktop\Encryption_API\Curl\file_to_upload.txt http://127.0.0.1:5000/create_secure_ptr`   
5  | Postman will return a password and create the zipped file inside a folder that has the name of the PTR number(The folder will be created inside a folder named Encrypted_ZIP , in the folder where api.py is located).

