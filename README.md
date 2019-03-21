# Sublime Text Settings
Mi configuracion estandar de Sublime Text 3.
Con múltiples funcionalidades, snippets, colorSchemes, temas personalizados, WordPress completions y Snippets anadidos de PHP.

### Si desea ver mi coniguracion de Sublime Text, paquetes y snippets, clone o descargue el repositorio.

### Extra - XAMPP MAIL

You can send mail from localhost with sendmail package , sendmail package is inbuild in XAMPP. So if you are using XAMPP then you can easily send mail from localhost.

for example you can configure C:\xampp\php\php.ini and c:\xampp\sendmail\sendmail.ini for gmail to send mail.

in C:\xampp\php\php.ini find extension=php_openssl.dll and remove the semicolon from the beginning of that line to make SSL working for gmail for localhost.

in php.ini file find **mail function** and change

SMTP=smtp.gmail.com
smtp_port=587
sendmail_from = my-gmail-id@gmail.com
sendmail_path = "\"C:\xampp\sendmail\sendmail.exe\" -t"


Now Open C:\xampp\sendmail\sendmail.ini. Replace all the existing code in sendmail.ini with following code

**sendmail**

smtp_server=smtp.gmail.com
smtp_port=587
error_logfile=error.log
debug_logfile=debug.log
auth_username=my-gmail-id@gmail.com
auth_password=my-gmail-password
force_sender=my-gmail-id@gmail.com
Now you have done!! create php file with mail function and send mail from localhost.


