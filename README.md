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


## Donate
If this project help you reduce time to develop, you can give me a cup of coffee to continue its development. Thank you! :)
[![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=6G2KF2TWFFEA6)
