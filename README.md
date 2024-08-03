# Agora On Chain - Technical Inception

## Componentes centrales

- Backend wallets / Account Abstraction ([ThirdWeb](https://portal.thirdweb.com/connect/account-abstraction/overview))
- Minimal Anti-Collusion Infrastructure ([MACI](https://maci.pse.dev/))

## User Jouney y Arquitectura

El usuario se registra en AGORA utilizando login clásico social web2 (Gmail, Facebook, Etc) o login web 3
 
Aquellos usuarios que eligen conectarse con plataformas web2 tendrán por detrás gestionada una wallet sin que deban hacer nada. Este es un primer salto de UX para aquellos espacios y usaurios que no conocen web3.

<img width="715" alt="image" src="https://github.com/user-attachments/assets/7fc10fdb-8b35-4537-9ea5-622457946d7e">

En la plataforma podrán acceder a distintos espacios que nuclean votaciones. Cada espacio tiene sus propios criterios de participación.

<img width="698" alt="image" src="https://github.com/user-attachments/assets/724522b1-78df-4be5-94b3-2074423fd3f9">

Para ejecutar la votación propiamente dicha, se utilizará MACI. Se desplegarán los smart-contracts, teniendo a Agora como coordinator.


