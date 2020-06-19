## Installer les dépendences (PHPMailler) :
`composer install`
  
## Email service
Create a free account on [SendGrid](https://sendgrid.com/).  
Create a [Single Sender Verification](https://sendgrid.com/docs/ui/sending-email/sender-verification/).  
Under the tab `Email API` -> `Integration Guide` choose SMTP Relay and `Create Key`.
  
## Rentrer la clé api de sendGrid
Dans `index.php` a la ligne 21 il faut remplacer `'api_key_from_send_grid'`
  
## Renseigner les email
Dans `index.php` a la ligne 26 il faut metre le mail sur lequel tu a fait le `Single Sender Verification`.  
Dans `index.php` a la ligne 27 c'est l'email du destinataire.

## Executer le script
`php index.php`