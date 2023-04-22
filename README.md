<div align="center">
  
<h1 style="bottom-border:none;"> <b> decentralized-supply-chain-network </b> </h1>
 
  <a href="">![GitHub CI](https://img.shields.io/badge/build-passing-brightgreen)</a>
  <a href="">![GitHub CI](https://img.shields.io/badge/network--version-0.0.1-blue)</a>
  <a href="">![GitHub CI](https://img.shields.io/badge/network--card-failed-red)</a>
  <a href="">![GitHub CI](https://img.shields.io/badge/documentation-limited-yellow)</a>
  
This is a University Final Year Project.
	
</div>

Project Scope
------------------------------------------------------------------
The aim of this project is to develop a web-based decentralized supply-chain management system that leverages the benefits of blockchain technology to ensure transparency, security, and accountability throughout the entire supply chain. The system will be designed to be user-friendly and easily accessible to all stakeholders involved in the supply chain process.
It will involve different participants who will be able to create purchase orders to purchase commodities. Participants can initiate a purchase order for the commodity, and the commodity will be transferred between participants through two transactions. Two transactions will be involved in this process - the initiation of a purchase order and the transfer of the commodity based on the purchase order. The network will be built using Hyperledger composer Business Network which can be deployed at supported runtimes. 

Technological Requirements
------------------------------------------------------------------
### Hardware configuration

#### Deployment Platform
-	**Processor** : Intel Core i5 or equivalent
-	**Memory (RAM)** : 16GB or more
-	**Storage** : 250 GB or more solid-state drive (SSD)
-	**Operating System** : Windows 10 or later, MacOS X 10.12 or later, or a Linux distribution
-	**Network** : A stable and fast internet connection

#### Development Platform
-	**Processor** : Intel i5 13th Gen or equivalent
-	**Memory** : 8 GB RAM
-	**Storage** : 250 GB hard disk
-	**Operating System** : Ubuntu Linux 16.04 (both 64-bit) or Mac OS X 10.12.6 
-	Internet connection

### Software configuration

#### Deployment Platform
-	**Node.js and NPM (Node Package Manager)** : npm v5 to be installed, & node accordingly.
-	**Yeoman generator** : You can install it using the NPM command ```npm install -g yo@2.0.5 ```
-	**Hyperledger Composer** : You can install it from the official Hyperledger Composer website ```npm generator-hyperledger-composer@0.20.9 ```
-	**Composer CLI & Playground** : You can install it using the NPM command ```npm install -g generator-hyperledger-composer composer-cli composer-playgrouund ```
-	**Internet connectivity** : You need to have an active internet connection to install the required dependencies and packages.
-	**Web Browser** : A modern web browser like Google Chrome, Firefox or Safari, for testing and debugging the REST API (npm composer-rest-server@0.20.9).

#### Development Platform
-	**Docker Engine** : Version 17.03, build f0df350
-	**Docker-Compose** : Version 1.13.0, build 1719ceb
-	**Node** : v8.9.4 (Note: v9 is not supported)
-	**npm** : v5.6.0
-	**git** : 2.9.x or higher
-	**Python** : 2.7.12
-	VS Code or/and Hyperledger Composer Playground

*// [TLDR for Installation of Dependencies](https://medium.com/@aka.0x4C3DD/hyperledger-composer-playground-a-fresh-installation-guide-on-linux-vm-e457e04cf5ab)*

## Requirement Design

<div align="center">

![requirement-design.png](https://github.com/aka-0x4C3DD/SupplyChainNetwork-6thSemProject/blob/main/support/requirement-design-ve.png)

</div>

**Participants**: Supplier, Manufacturer, Distributor, Retailer, Consumer Assets: Commodity, Purchase Order
**Transactions**: Initiate Purchase Order, Transfer Commodity

Logic –
- **Initiate Purchase Order**: When a participant calls this transaction a new asset is created under Purchase Order this entry includes the demanded items, their supporting accessories, the supplier etc.
- **Transfer Commodity**: When this transaction is called a new owner is assigned to the commodity based on the stage and is called against purchase order.

Based on the above diagram we will create a business network structure based on all the initial participants in mind. Define it and generate archive files for the same using the composer. Then we will deploy the business network over a runtime environment which will include Hyperledger fabric, web and embedded NodeJS for the convenient access by the stakeholders.

Screenshots
------------------------------------------------------------------

<div align="center">

![install.png](https://github.com/aka-0x4C3DD/SupplyChainNetwork-6thSemProject/blob/main/support/Ubuntu%2064-bit%20%5B16.04-Playground%5D-2023-04-12-08-08-14.png)

![install.png](https://github.com/aka-0x4C3DD/SupplyChainNetwork-6thSemProject/blob/main/support/Ubuntu%2064-bit%20%5B16.04-Playground%5D-2023-04-12-08-09-29.png)

![prod.png](https://github.com/aka-0x4C3DD/SupplyChainNetwork-6thSemProject/blob/main/support/VirtualBox_Ubuntu_Xenial-Xerus_16.4.7_amd64_12_04_2023_08_14_42.png)	

![test.png](https://github.com/aka-0x4C3DD/SupplyChainNetwork-6thSemProject/blob/main/support/VirtualBox_Ubuntu_Xenial-Xerus_16.4.7_amd64_12_04_2023_08_16_29.png)

![test.png](https://github.com/aka-0x4C3DD/SupplyChainNetwork-6thSemProject/blob/main/support/VirtualBox_Ubuntu_Xenial-Xerus_16.4.7_amd64_12_04_2023_08_15_32.png)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
