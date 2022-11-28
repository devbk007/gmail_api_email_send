![Image](https://user-images.githubusercontent.com/43404287/172422574-9f1bf25f-0286-40f7-8e38-a0423a594b74.png)

# Send email using python with Google Email API

1. Create a virtual enviroment
    If using conda , install using the command 
    
    ```
    conda create --prefix ./envs
    ```

2. Activate virtual environment
    ```
    conda activate ./envs
    ```

3. Install following packages
    ```
    pip install --upgrade google-api-python-client google-auth-httplib2 google-auth-oauthlib
    ```

4. Create a project, in Google accounts, setup OAuth consent screen and create an OAuthID. 
    [![Watch the video for step by step setup]](https://youtu.be/6bzzpda63H0)   

5. Add a test user in the OAuth consent screen with the required email id.
6. Enable the Gmail API.
7. Download the credentials as Json file and save as client_secret.json in the project directory.
8. Add recipient email id by replacing '<recipient_email_id>' in line 16, message in line 14 and subject in line 17 of send_email.py.
9. Run the command python send_email.py. A prompt screen will appear, if running for the first time. Configure by using the test user email id given in step 5.

#### Tip
If refresh error occur, then delete the token files and rerun.
