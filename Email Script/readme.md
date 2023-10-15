# Email Sending Script

This is a simple Python script to send emails using SMTP. 

## Usage

Update the following variables in the script:

- `email` - The email address to send from
- `password` - The password for the email address
- `recipient` - The recipient's email address
- `SMTP_SERVER_ADDRESS` - The SMTP server address. For Gmail this is `smtp.gmail.com`

Run the script:

```
python singleEmailSernder.py
```

An email will be sent to the recipient address with the subject "Test Subject" and plain text body "This is a test email".

## Libraries Used

- smtplib - Used for connecting to the SMTP server and sending the email
- SSL - Used for creating a SSL context to connect securely 
- MIMEMultipart - Used for constructing the email message with text and attachments
- MIMEText - Used for the text body of the email message

## How it Works

- Connects to the SMTP server using SSL 
- Logs in with the provided username and password
- Constructs the email message with recipient, subject, and plaintext body
- Sends the message
- Prints the response code and message from the server 
- Closes the connection

So in summary, this script provides a simple way to send automated emails using Python by connecting to an SMTP server.