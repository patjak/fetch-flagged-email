# fetch-flagged-email
This project was developed to ease downloading and applying git patches from gmail. Simply "star" the patch email, apply a label (or leave in your inbox), and run the python script. The starred patches will be downloaded and stored in a folder with consecutive numbers based on their arrival times for easy processing using git-am.

The functionality is not patch-specific: any "starred" email will be downloaded and saved. If you find this useful +1 and star to your left.

fetch-flagged-email.py retrieves email that has been \\Flagged (gmail starred). Specify a folder (gmail label) and it will retrieve all flagged emails in that folder using imap and your account/password. The imap support relies on a non-standard python library imapclient which is available at http://imapclient.freshfoo.com/. Emails are saved in text files based on email sequence numbers. You also need to enable IMAP in gmail. 
