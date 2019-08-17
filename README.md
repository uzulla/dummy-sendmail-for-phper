# Dummy sendmail

output STDIN to file.

## require

php(>=7)

## usage

#### if you use `mail`/`mb_send_mail`.

```
# in php.ini
sendmail = "/path/to/dummy-sendmail-for-phper/sendmail -d /path/to/some/writable_dir -t"
```

or 

```
# in code
ini_set("sendmail", "/path/to/dummy-sendmail-for-phper/sendmail -d /path/to/some/writable_dir -t");
```

and go on

#### if you use Swiftmailer(or other)

```
# in code
$transport = new Swift_SendmailTransport('/path/to/dummy-sendmail-for-phper/sendmail -d /path/to/some/writable_dir -t');
```


## check output

Open `*.eml` file with editor(eml is RAW mime text, difficult to read) or some mail client (ex: mail.app, thunderbird). 


## LICENSE

MIT


