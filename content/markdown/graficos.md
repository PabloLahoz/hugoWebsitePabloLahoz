+++
date = '2024-11-21T18:31:41+01:00'
draft = false
title = 'Graficos Mermaid'
type = 'post'
+++

#### Para este apartado se ha debido modificar el tema añadiendo un script a head.html y crear un shortcode mermaid.html en la carpeta layouts.

## Diagrama de flujo

Para crear un diagrama de flujo se puede usar ```graph``` o ```flowchart```

También puedes orientarlo:
- TB - De arriba al fondo
- TD - De arriba a abajo
- BT - Del fondo a arriba
- RL - De derecha a izquierda
- LR - De izquierda a derecha
```
flowchart BT
navegador --Llama--> B[Servidor web]
A --> B
A --> C
B --> C
C --> D
```
### Se verá:
{{< mermaid >}}
flowchart BT
navegador --Llama--> B[Servidor web]
A --> B
A --> C
B --> C
C --> D
{{< /mermaid >}}

## Gráfico circular
```
pie title Actividades
        "Dormir" : 34
        "Instituto" : 25
        "TV" : 8
        "Jugar" : 8
        "Música" : 25
```
### Se verá:
{{< mermaid >}}
pie title Actividades
        "Dormir" : 34
        "Instituto" : 25
        "TV" : 8
        "Jugar" : 8
        "Música" : 25
{{< /mermaid >}}

## Diagrama de secuencia
```
sequenceDiagram
    participant Usuario
    participant Servidor
    Usuario->>Servidor: Solicita recurso
    Servidor-->>Usuario: Devuelve recurso
```
### Se verá:
{{< mermaid >}}
sequenceDiagram
    participant Usuario
    participant Servidor
    Usuario->>Servidor: Solicita recurso
    Servidor-->>Usuario: Devuelve recurso
{{< /mermaid >}}
