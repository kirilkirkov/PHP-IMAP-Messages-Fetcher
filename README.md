# PHP IMAP 
Retrieve messages from an IMAP server

## Usage example:
```
$imap = new Imap();
$connection_result = $imap->connect('{imap.gmail.com:993/imap/ssl}INBOX', 'user@gmail.com', 'password');
    if ($connection_result !== true) {
        echo $connection_result; //Error message!
        exit;
    }
$messages = $imap->getMessages('text'); //Array of messages
```
#### in $attachments_dir property set directory for attachments
#### in the __destructor set errors log file
