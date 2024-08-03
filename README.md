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

## Proof of Concept

Se realizó un deploy en Scroll-Sepolia de los smart-contracts de MACI junto a los smart-contracts de una poll:

```
	ConstantInitialVoiceCreditProxy: 0xb5B39344b8d2b706aE55Fe10e996C1A357A1C394
	ZupassGatekeeper: 0x5E998b32E5EE401a047320eACBb4eEa00DaCcfF8
	Verifier: 0x71e3e21a102B9164B94F36c4A9f52B5ce4FefA18
	PoseidonT3: 0xb5fb5dB6556b9f9714F89bDeF4362163Da066F11
	PoseidonT4: 0xE52A76bEEdAb4CbcD8F0bc6E17F1Ae198cb931B8
	PoseidonT5: 0xC8576Ee1073919c67F009d503d4953BbD6121aeA
	PoseidonT6: 0x99CCf4175ea0E39b4255A711F6146B73ade5c230
	PollFactory: 0x579EeF94712Af1A0aBB24bf494fF905022E07850
	MessageProcessorFactory: 0x1ec34A48CBBfd29E8686EdA93F9eC055Bb5F15AF
	TallyFactory: 0xa89DaC4499b4Fc6920691162cD437D40c7B92bD8
	MACI: 0xc4588A5bF457F8A2E141d76D2Bfed91262F44194
	VkRegistry: 0xBe84712A0D61C5E576300539F3aA5FE7c747AF4f
	Poll-poll-0: 0xbB461F57B99B64aCBfaBdE29C0f82fc9e78b6899
	MessageProcessor-poll-0: 0x478bF6aF745d164e5De7a3f174188E39ce28e693
	Tally-poll-0: 0xFE3358b48C5A0c643CB124D88c631452Cc9DbFa9
	AccQueueQuinaryMaci-poll-0: 0x6c5272BadA08bA051805149E22222734592Ce27D
```
