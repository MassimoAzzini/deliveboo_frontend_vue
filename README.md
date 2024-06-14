Deliveboo Frontend 
===

Questa web-app è composta da una parte back-end (deliveboo_backend_laravel) scritta in PHP utilizzando il framework Laravel10 e da una parte front-end (deliveboo_frontend_vue) scritto con l'utilizzo del framework Vue3.
Lato back-end vengono utilizzate delle query ad un database MySQL per il recupero dei dati dei ristoranti e prodotti.
Il front-end comunica con il back-end tramite Axios.
Tutta l'applicazione è completamente responsive quindi utilizzabile da tutti i dispositivi.

PER PROVARE QUESTA APP E' NECESSARIO:

### DELIVEBOO BACKEND
- Scaricare o Clonare sul vosto editor di codice deliveboo_backend_laravel
- lanciare dal terminale il comando: composer install
- dupplicare il file .envexemple e rinominarlo .env
- lanciare dal terminale il comando: php artisan key:generate
- lanciare dal terminale il comando: npm install

- siccome all'interno del progetto c'e' uno storage publico bisogna:
  - lanciare dal terminale il comando: php artisan storage:link
  - nel file .env impostare FILESYSTEM_DISK=public
  - nel file filesystems.php nella cartella config verificare che ci sia impostato:   'default' => env('FILESYSTEM_DISK', 'public'),

- completare l'impostazione del file  .env con i dati del vostro database
- copiare tutta la cartella upload qui linkata all'interno della cartella storage/app/public: https://drive.google.com/file/d/1vmoSZMjJ2JNIBAzCQRbDPddut9whkZgq/view?usp=drive_link


- per popolare il vostro DB con ristoranti e prodotti di prova lanciare dal terminale i seguenti comandi: 
    - php artisan migrate
    - php artisan db:seed

- lanciare dal terminale il comando: npm run dev
- lanciare dal terminale il comando: php artisan serve

***

### DELIVEBOO FRONTEND
- Scaricare o Clonare sul vosto editor di codice deliveboo_frontend_vue
- lanciare dal terminale il comando: npm install

(prima di procedere con questo passaggio deve essere lanciato DELIVEBOO BACKEND come da indicazioni precedenti)
- lanciare dal terminale il comando: npm run dev
cliccare il link del localhost per lanciare l'app.

***

Per vedere la dashboard del ristorante inserire nel login i seguenti valori:
- email: cerinodoro@gmail.com
- psw: 123123123

