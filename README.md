# WebminM4
Un repositori pel Mòdul 4 de SMX ; en colaboració amb el gran Dani Agache.

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
  ![image](https://github.com/user-attachments/assets/d592942e-4115-44c3-89db-c335685dfc22)

- Des de webmin actualitza un paquet.
  ![image](https://github.com/user-attachments/assets/9139c343-0d99-4deb-94d0-5068fed83504)
  ![image](https://github.com/user-attachments/assets/ef84924a-581c-4719-abe5-b750dbfe757e)

- Utilitza webmin per instal·lar un joc de apt.
  ![image](https://github.com/user-attachments/assets/198a64b4-b839-401e-93a7-e174a7f17403)
  ![image](https://github.com/user-attachments/assets/1dadfa95-321d-4871-b620-0db7b6f09ba0)
  
- Utilitza webmin per instal·lar gimp de apt.
  ![image](https://github.com/user-attachments/assets/9792d472-e8c0-4453-8896-93353cf9268e)
  ![image](https://github.com/user-attachments/assets/00bfb3c5-afc6-46fe-9658-a6479206692d)

- Utilitza webmin per desinatl·lar el joc que heu instal·lat abans.
  ![image](https://github.com/user-attachments/assets/ab2446f4-e13d-439a-ab31-bed2500b517d)
  ![image](https://github.com/user-attachments/assets/f1fcbdb9-8570-4fe0-ae12-00b3ad25032c)
  ![image](https://github.com/user-attachments/assets/d413c7f9-e252-4d66-bd36-7a743bcc3a13)

  
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
![image](https://github.com/user-attachments/assets/b41088b0-10ef-40be-9d46-9891104d1750)

- Utilitza webmin perquè l'usuari bakalao_X no pugui tenir més de 2 MB d'informació al disc.
  ![image](https://github.com/user-attachments/assets/7fb63303-a67b-4d25-a42c-3289c19d6ff9)
  ![image](https://github.com/user-attachments/assets/3a8cf31a-e8ea-413c-aa07-ca2bd3d4563f)

- Comprova que el límit de la quota funciona.
  ![image](https://github.com/user-attachments/assets/044581d3-3cca-4faa-bdf3-5a5b1e1bb872)
  
- Utilitza webmin perquè l'usuari techno no pugui tenir més de 10 fitxers al disc.
  ![image](https://github.com/user-attachments/assets/9657f417-8947-4106-91cc-962827b9c20d)

- Comprova que el límit de la quota funciona.
  ![image](https://github.com/user-attachments/assets/df58be12-9161-4d7d-b535-30933e7efd86)

## 6.- Còpies de seguretat

- Utilitzant el mòdul de Webmin Filesystem Backup fes una còpia de seguretat del directori /home al directori /backups (l'haureu de crear si no existeix).
- Modifica alguns fitxers de /home.
- Recupera la còpia de seguretat.
- Comprova que els fitxers de /home són els correctes.
- Programa una còpia de seguretat de /home/bakalao_X per els divendres a les 21:00.
- Esborra la còpia de seguretat programada anteriorment.

## 7.- Compartició

- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "area_public_X" per a usuaris sense autenticar en forma de lectura i escriptura.
  ![image](https://github.com/user-attachments/assets/a5eb3264-93f1-45cc-9a1c-2af61b0b4851)

- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "pontaeri_privat_X" per a usuaris _X i techno només de lectura.
  
- Comprovar des de Windows que aquests recursos funcionen.

# Grups:

1. Kristopher i Eric
2. Oscar i Nil
3. Oriol i Ayoub
4. Arno i Daniel
5. Sebastian i Biel
