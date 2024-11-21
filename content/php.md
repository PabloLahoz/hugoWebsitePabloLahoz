+++
date = '2024-11-21T23:29:36+01:00'
draft = false
title = 'Php'
type = 'page'
+++

## Imprimir texto
Para imprimir texto con php se usan echo, print, printf, print_r y var_dump.
```php
<?php
echo "¡Hola Mundo!";
print "¡Hola Mundo!";
$n = 78.2342923;
printf("El valor con 3 decimales es %.2f",$n);
$array = array("BMW","Opel","Audi","Toyota");
print_r($array);
var_dump($n);
var_dump($array);
?>
```

## Variables y tipos de datos
En php, las variables se identifican con el símbolo ```$``` seguido del nombre.
```php
<?php
$nombre = "Pablo"; // String
$edad = 25;        // Entero
$precio = 19.99;   // Flotante
$esActivo = true;  // Booleano

echo "Hola, mi nombre es $nombre y tengo $edad años.";
?>
```

## Condicionales
Las estructuras ```if-else``` permiten ejecutar código en función de si una condición es verdadera o falsa.
```php
if ($edad >= 18) {
    echo "Eres mayor de edad.";
} else {
    echo "Eres menor de edad.";
}
```
