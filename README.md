# Kaggle
# Setting up Kaggle API on Mac OS



1. Installing the library

Launch Terminal on Mac OS
Using the command pip install kaggle
Using the command pip install --user kaggle


2. Setting up the API token

Go to the kaggle website.
Click on Your profile button on the top right and then select My Account.
Scroll down to the API section and click on the Create New API Token button.
It will initiate the download of a file call kaggle.json to /Downloads on your machine.

3. place the .json file at the correct location
Create .kaggle folder in your home directory and move downloaded JSON file to /.kaggle

mkdir ~/.kaggle
cd 
mv Downloads/kaggle.json ~/.kaggle/kaggle.json
or mv Download/kaggle.json ~/.kaggle

./kaggle is hidden. To see this folder, press simultaneously shift + cmd + .

4. Give proper permissions to the file (since this is a hidden folder):

chmod 600 ~/.kaggle/kaggle.json

5. Checking if it works

~/.local/bin/kaggle competitions list

5. Using the API

Sources: 
https://www.kaggle.com/docs/api#getting-started-installation-&-authentication
https://adityashrm21.github.io/Setting-Up-Kaggle/
