# WebminM4
Un repositori pel Mòdul 4 de SMX ; en colaboració amb el gran Dani Agache

# Utilitzant webmin per administrar el servidor

- Entregueu link a un repositori **públic** (un link per alumne) de Github on feu les següents tasques.
- Expliqueu el que feu amb text i captures.
- **Fer tot des de webmin**
- Rúbrica:
  - 2 punts - Estructura del document (portada, índex, captures correctes, text ben formatat...).
  - 1 punt - Exercici 1.
  - 1 punt - Exercici 2.
  - 1 punt - Exercici 3.
  - 1 punt - Exercici 4.
  - 1.5 punt - Exercici 5.
  - 1.5 punt - Exercici 6.
  - 1 punt - Exercici 7.

## 1.- Crear i modificar usuaris

**Fer tot des de webmin**

- Has de crear dos usuaris bakalao_X i techno_X on (X és el vostre cognom).
  ![image](https://github.com/user-attachments/assets/08e96e9b-706f-42be-a1e6-cf033a7b6cdf)
  ![image](https://github.com/user-attachments/assets/a51537f4-59bd-4f75-9c9b-26874756a7d5)
  
- Els usuaris et passaran el hash de la seva contrasenya, no la contrasenya real. (podeu fer servir openssl).
  ![image](https://github.com/user-attachments/assets/201192f4-7af2-49eb-91ab-3b69c0bdad17)
  ![image](https://github.com/user-attachments/assets/46289de0-5284-47a2-bbcc-26933cab5508)
  ![image](https://github.com/user-attachments/assets/b2bd7a51-f38d-44a2-899d-9540c9b46732)

- Cada usuari tindrà un directori a home igual al seu nom d'usuari.
  ![image](https://github.com/user-attachments/assets/cd1c0bfd-6c2d-4e8c-829b-c2f45dfe0363)

- Utilitzaran bash com a shell.
  ![image](https://github.com/user-attachments/assets/17223d95-cf1e-4427-953a-4a3f6414e228)
  ![image](https://github.com/user-attachments/assets/4a1896e9-6db3-450b-b1e7-d072883b96f6)

- Els usuaris estaran dins del grup que tingui el seu mateix nom i dins del grup usuaris_empresa.
  ![image](https://github.com/user-attachments/assets/f102af6a-f8e0-4dd5-9742-7886f56e7f28)

- L'usuari techno no podrà fer login després del dia 31-03-2025.
  ![image](https://github.com/user-attachments/assets/13cbd3f6-da25-4165-9d69-7c354cc3a744)

- Comproveu que els usuaris poden iniciar sessió. <br>
  ![image](https://github.com/user-attachments/assets/d68a3d7a-ce28-4770-8466-8762328d61fa)

- Canvia la data del sistema (utilitzant webmin) i comprova que techno no pot iniciar sessió si estem a dia 01-04-2025.
  ![image](https://github.com/user-attachments/assets/6368e592-868c-4930-b646-21a3e3d6ed6b)
  ![image](https://github.com/user-attachments/assets/a2b2d808-e997-4f64-87a5-b9b9c8b02775)
  ![image](https://github.com/user-attachments/assets/0528475c-2cc0-481a-8953-1941bb585703)



## 2.- Programar tasques

- Programa una tasca que neteja els paquets de Linux que ja no s'utilitzen una vegada al mes.
- Programa una tasca diaria que apaga l'ordinador a les 14:00.
- Comprova que funcionen (canvia dia i hora del sistema mitjançant webmin).
  
## 3.- Instal·lació de software

- Utilitza webmin per mostrar quins paquets de software es podrien actualitzar.
- Des de webmin actualitza un paquet.
- Utilitza webmin per instal·lar un joc de apt.
- Utilitza webmin per instal·lar gimp de apt.
- Utilitza webmin per desinatl·lar el joc que heu instal·lat abans.

## 4.- Serveis

- Utilitza webmin per mostrar els serveis que s'inicien amb el sistema.
- Utilitza webmin per mostrar els serveis que estan actius.
- Utilitza webmin per mostrar l'estat del servidor Apache.
- Utilitza webmin per aturar Apache.
- Utilitza webmin per mostrar l'estat del servidor Apache apagat.
- Utilitza webmin per reiniciar Apache.
- Utilitza webmin per mostrar l'estat del servidor Apache reiniciat.

## 5.- Quotes de disc

Activa les quotes de disc pels usuaris amb la comanda: 

```
sudo apt install quota quotatool
```

- Utilitza webmin perquè l'usuari bakalao_X no pugui tenir més de 2 MB d'informació al disc.
- Comprova que el límit de la quota funciona.
- Utilitza webmin perquè l'usuari techno no pugui tenir més de 10 fitxers al disc.
- Comprova que el límit de la quota funciona.

## 6.- Còpies de seguretat

- Utilitzant el mòdul de Webmin Filesystem Backup fes una còpia de seguretat del directori /home al directori /backups (l'haureu de crear si no existeix).
- Modifica alguns fitxers de /home.
- Recupera la còpia de seguretat.
- Comprova que els fitxers de /home són els correctes.
- Programa una còpia de seguretat de /home/bakalao_X per els divendres a les 21:00.
- Esborra la còpia de seguretat programada anteriorment.

## 7.- Compartició

- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "area_public_X" per a usuaris sense autenticar en forma de lectura i escriptura.
- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "pontaeri_privat_X" per a usuaris _X i techno només de lectura.
- Comprovar des de Windows que aquests recursos funcionen.

# Grups:

1. Kristopher i Eric
2. Oscar i Nil
3. Oriol i Ayoub
4. Arno i Daniel
5. Sebastian i Biel
