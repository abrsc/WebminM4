# WebminM4
Un repositori pel Mòdul 4 de SMX ; en colaboració amb el gran Dani Agache.

# Webmin
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9d/Webmin_Logo.svg/2048px-Webmin_Logo.svg.png" alt="webmin" width="200"/>

## Índex
 * [1.- Crear i modificar usuaris](#1)
 * [2.- Programar tasques](#2)
 * [3.- Instal·lació de software](#3)
 * [4.- Serveis](#4)
 * [5.- Quotes de disc](#5)
 * [6.- Còpies de seguretat](#6)
 * [7.- Compartició](#7)

<a id="1"></a>
## 1.- Crear i modificar usuaris

**Fer tot des de webmin**

- Has de crear dos usuaris bakalao_X i techno_X on (X és el vostre cognom).
  ![image](https://github.com/user-attachments/assets/428d5704-5b4c-4eed-848e-bebe6fcd5c85)
  ![image](https://github.com/user-attachments/assets/08e96e9b-706f-42be-a1e6-cf033a7b6cdf)
  ![image](https://github.com/user-attachments/assets/a51537f4-59bd-4f75-9c9b-26874756a7d5)
  
- Els usuaris et passaran el hash de la seva contrasenya, no la contrasenya real. (podeu fer servir openssl).
  ![image](https://github.com/user-attachments/assets/201192f4-7af2-49eb-91ab-3b69c0bdad17)
  ![image](https://github.com/user-attachments/assets/46289de0-5284-47a2-bbcc-26933cab5508)
  ![image](https://github.com/user-attachments/assets/b2bd7a51-f38d-44a2-899d-9540c9b46732)

- Cada usuari tindrà un directori a home igual al seu nom d'usuari.
  ![image](https://github.com/user-attachments/assets/cd1c0bfd-6c2d-4e8c-829b-c2f45dfe0363)

- Utilitzaran bash com a shell. <br>
  Por la dreta a shell, seleccionar "bin/bash".
  ![image](https://github.com/user-attachments/assets/17223d95-cf1e-4427-953a-4a3f6414e228)
  ![image](https://github.com/user-attachments/assets/4a1896e9-6db3-450b-b1e7-d072883b96f6)

- Els usuaris estaran dins del grup que tingui el seu mateix nom i dins del grup usuaris_empresa.
  ![image](https://github.com/user-attachments/assets/5cea2281-3d59-4c11-843a-fef69848eebf)
  ![image](https://github.com/user-attachments/assets/4d983796-32dc-4676-a451-38886da213c8)
  ![image](https://github.com/user-attachments/assets/f102af6a-f8e0-4dd5-9742-7886f56e7f28)

- L'usuari techno no podrà fer login després del dia 31-03-2025.
  ![image](https://github.com/user-attachments/assets/13cbd3f6-da25-4165-9d69-7c354cc3a744)

- Comproveu que els usuaris poden iniciar sessió. <br>
  ![image](https://github.com/user-attachments/assets/d68a3d7a-ce28-4770-8466-8762328d61fa)

- Canvia la data del sistema (utilitzant webmin) i comprova que techno no pot iniciar sessió si estem a dia 01-04-2025.
  ![image](https://github.com/user-attachments/assets/6368e592-868c-4930-b646-21a3e3d6ed6b)
  ![image](https://github.com/user-attachments/assets/a2b2d808-e997-4f64-87a5-b9b9c8b02775)
  ![image](https://github.com/user-attachments/assets/0528475c-2cc0-481a-8953-1941bb585703)

<a id="2"></a>
## 2.- Programar tasques

- Programa una tasca que neteja els paquets de Linux que ja no s'utilitzen una vegada al mes.
    
    ![image.png](image.png)
    
    ![image.png](image%201.png)
    
- Programa una tasca diaria que apaga l'ordinador a les 14:00.
    
    ![](https://github.com/user-attachments/assets/318fd00c-4986-438b-9e56-09f0e112a6fb)
    
- Comprova que funcionen (canvia dia i hora del sistema mitjançant webmin).
    
    ![image.png](image%202.png)
    
    ![image.png](image%203.png)
    
    ![image.png](image%204.png)
    
    ![image.png](image%205.png)
    
    ![image.png](image%206.png)

<a id="3"></a>
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

<a id="4"></a>
## 4.- Serveis

- Utilitza webmin per mostrar els serveis que s'inicien amb el sistema.
    
    ![image.png](image%207.png)
    
- Utilitza webmin per mostrar els serveis que estan actius.
    
    ![image.png](image%208.png)
    
- Utilitza webmin per mostrar l'estat del servidor Apache.
    
    ![image.png](image%209.png)
    
- Utilitza webmin per aturar Apache.
    
    ![image.png](image%2010.png)
    
- Utilitza webmin per mostrar l'estat del servidor Apache apagat.
    
    ![image.png](image%2011.png)
    
- Utilitza webmin per reiniciar Apache.
    
    ![image.png](image%2012.png)
    
- Utilitza webmin per mostrar l'estat del servidor Apache reiniciat.
    
    ![image.png](image%2013.png)

<a id="5"></a>
## 5.- Quotes de disc

Activa les quotes de disc pels usuaris amb la comanda: 

```
sudo apt install quota quotatool
```
![image](https://github.com/user-attachments/assets/b41088b0-10ef-40be-9d46-9891104d1750)

- Utilitza webmin perquè l'usuari bakalao_X no pugui tenir més de 2 MB d'informació al disc.
  ![image](https://github.com/user-attachments/assets/8461c630-6e28-410c-8646-e3f42c0e11e2)
  ![image](https://github.com/user-attachments/assets/1274aca0-f075-43ed-b7fb-7fff2715036c)
  ![image](https://github.com/user-attachments/assets/3a8cf31a-e8ea-413c-aa07-ca2bd3d4563f)

- Comprova que el límit de la quota funciona.
  ![image](https://github.com/user-attachments/assets/044581d3-3cca-4faa-bdf3-5a5b1e1bb872)
  
- Utilitza webmin perquè l'usuari techno no pugui tenir més de 10 fitxers al disc.
  ![image](https://github.com/user-attachments/assets/9657f417-8947-4106-91cc-962827b9c20d)

- Comprova que el límit de la quota funciona.
  ![image](https://github.com/user-attachments/assets/df58be12-9161-4d7d-b535-30933e7efd86)

<a id="6"></a>
## 6.- Còpies de seguretat

- Utilitzant el mòdul de Webmin Filesystem Backup fes una còpia de seguretat del directori /home al directori /backups (l'haureu de crear si no existeix).
    
    ![image.png](image%2014.png)
    
    ![image.png](image%2015.png)
    
    ![image.png](image%2016.png)
    
    ![image.png](image%2017.png)
    
- Modifica alguns fitxers de /home.
    
    ![image.png](image%2018.png)
    
- Recupera la còpia de seguretat.
    
    ![image.png](image%2019.png)
    
    ![image.png](image%2020.png)
    
    ![image.png](image%2021.png)
    
    ![image.png](image%2022.png)
    
- Comprova que els fitxers de /home són els correctes.
    
    ![image.png](image%2023.png)
    
- Programa una còpia de seguretat de /home/bakalao_X per els divendres a les 21 :00.
    
    ![image.png](image%2024.png)
    
    ![image.png](image%2025.png)
    
- Esborra la còpia de seguretat programada anteriorment.
    
    ![image.png](image%2026.png)

<a id="7"></a>
## 7.- Compartició
- Primer pas, convertir als usuaris a usuaris de Samba.
  ![image](https://github.com/user-attachments/assets/46e86ce7-0284-48f3-9b1f-6506b470f56a)
  ![image](https://github.com/user-attachments/assets/fd0f8f82-e621-4112-9349-ca23bd4e0c55)

- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "area_public_X" per a usuaris sense autenticar en forma de lectura i escriptura.
  ![image](https://github.com/user-attachments/assets/0cd24091-86d7-45ad-97d1-0223af27784a)
  ![image](https://github.com/user-attachments/assets/6c90d1b4-a563-402a-ad32-5d624627994f)
  ![image](https://github.com/user-attachments/assets/3705f073-4707-4dfa-8055-7a1ac4c102a2)
  ![image](https://github.com/user-attachments/assets/c9492187-a667-46ec-88de-dad3be94aa50)

- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "pontaeri_privat_X" per a usuaris _X i techno només de lectura. <br>
  ![image](https://github.com/user-attachments/assets/cd7d1ed8-d85e-4b38-824a-54c2d9b0e7bc)
  ![image](https://github.com/user-attachments/assets/0e32da8f-20aa-4c60-9d99-3fce9e4c8340)
  ![image](https://github.com/user-attachments/assets/b907cc2e-b898-4436-9b70-d417a7174d90)
  ![image](https://github.com/user-attachments/assets/bc5ea726-a69c-45b2-93e6-cfd315f01b51)
  ![image](https://github.com/user-attachments/assets/6989b76b-2718-431d-91e7-4ba37f20af49)

- Comprovar des de Windows que aquests recursos funcionen. <br>
  #### Area Public:
  ![image](https://github.com/user-attachments/assets/9dc07f63-1b6e-47e5-9b83-fe82aab5b0f1)
  ![image](https://github.com/user-attachments/assets/336172eb-e2cb-4d9c-929d-3c99e815bb37)

  #### Pontaeri Privat: <br>
  Sessió com bakalao:
  ![image](https://github.com/user-attachments/assets/710c8a63-209b-49ae-896e-c26d70087c3f)

  Sessió com techno:
  ![image](https://github.com/user-attachments/assets/7608664d-48e0-4074-a1ae-31d18fffdce7)


# Grups:

1. Kristopher i Eric
2. Oscar i Nil
3. Oriol i Ayoub
### 4. Arno i Daniel
5. Sebastian i Biel
