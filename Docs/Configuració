## Configuració de la base de dades

1. Iniciar MySQL i accedir com a root:
   
    sudo mysql -u root -p
   

2. Crear la base de dades i usuari:
   
    CREATE DATABASE projectedb;
    CREATE USER 'lukaweb'@'localhost' IDENTIFIED BY 'Luka1234!';
    GRANT ALL PRIVILEGES ON projectedb.* TO 'lukaweb'@'localhost';
    FLUSH PRIVILEGES;
   


## Configuració d’Apache, PHP i permisos

Crear fitxer de configuració per a la connexió amb la base de dades a /var/www/html/config.php:
   
    <?php
    $host = "127.0.0.1";
    $db = "projectedb";
    $user = "lukaweb";
    $pass = "Luka1234!";
    $conn = new mysqli($host, $user, $pass, $db);
    if ($conn->connect_error) {
        die("Connexió fallida: " . $conn->connect_error);
    } else {
        echo "Connexió a la BBDD correcta";
    }
    ?>
   


Assignar permisos i propietari correctes per a la carpeta web:
   
    sudo chown -R www-data:www-data /var/www/html
    sudo chmod -R 755 /var/www/html
