# cloud-functions-ftp
This project is to create a ftp server. FTP listener will listen at ftp location and upload files to google bucket
- Put a file at FTP location.
- FTP listener listening to that location picks the file.
- FTP listener uploads the file in google storage bucket
- Cloud function is triggered on file upload.
- Cloud function downloads the csv file, converts it to json and pushes it to firebase and firebase queue.

## Install dependencies both in root and /functions
npm install

## Deploy functions
npm run deploy

### Running FTP server
node index.js

### Connecting to ftp
- ftp
- ftp> open
- ftp> 127.0.0.1
- ftp> <userName>
- ftp> <password>

### Google service account
Create service_account.json file at root location

### Create a google bucket ftp_demo

## Starting point
Put a csv file at FTP location by connecting to ftp server.

