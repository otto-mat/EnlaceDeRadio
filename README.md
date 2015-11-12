# EnlaceDeRadio

A laburar para un lindo tuto

A partir de la necesidad de radios comunitarias alternativas y popular es que nos pusimos a generar este tuto para tener un enlace via internet en el caso de que el estudio de la radio no esté donde está el transmisor de FM

Idea
Un script endemoniado que cuando se prenda la computadora cominence a reproducir el streaming de intrnet que tira la radio desde sus estudios. Esta contemplado que se el servidor de streaming, el estudio o la planta transmisora deja de funcionar, al momento de retomar es servicion, la radio vuelve al aire


###  otra ???IDEA
    Montar una interfaz web (mediante urls) que permita iniciar, reiniciar e incluso configurar la reproduccion de un streaming en una pc remota
    URLs:
        
#####  No se si esto vale la pena
        Sirve para dejar una computadora que esté todo el tiempo reproduciendo un streaming (posiblemente para salir al transmisor de radio), y que en caso de insterrupcion de las conexiones que se recomponga automaticamente. 

    http://IP:PUERTO/radio/start         (Inicia la reproduccion)
    http://IP:PUERTO/radio/stop          (Detiene la reproduccion)
    http://IP:PUERTO/radio/restart       (Reinicia la reproduccion)
    http://IP:PUERTO/radio/config/{url}  (Cambia la ulr a reproduccir)
    http://IP:PUERTO/radio/local         (Reproduce desde una determinada carpeta local)

INSTALAR:
    Debian u otro GNU/Linux con 
    Sistema operativo 
    
    #no se si ahce falta
    Bottle: Python Web Framework
    Es lo que permite crear el server y ejecturar acciones en base a las url y request
    
    MPlayer
    Es el programa utilizado para reproducir el streaming en la pc, será controlado por un script en python.
    
    DDClient, cron o similares
    Para manterner la IP del servidor actualizada con algun servicio de DDNS (FreeDNS por ejemplo)
    
    Requisito extra:
    Tener abierto y redireccionado un puerto desde el router para que se pueda acceder al servicio desde Internet

