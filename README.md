# CiviPort-Alpha
Alpha test of CiviPort V1 on the Kovan and Sokol Testnets

## Hello Admin how do I use this?

The very fist thing you need to do is download the CiviPort Client from [here](https://github.com/Civitas-Fundamenta/CiviPort-Alpha/releases). Make sure you pick the right download for your operating system.

The donwload is a zip file which will need to be extracted:

### Windows

After downloading navigate to the directory the zip file was downloaded to and right click the flie.  Choose `Extract All`.

![Extract1](https://github.com/Civitas-Fundamenta/CiviPort-Alpha/blob/main/extract1.png)

A window will pop up and ask you to choose the path of the extraction.  You can make this whatever you want.

![Extract2](https://github.com/Civitas-Fundamenta/CiviPort-Alpha/blob/main/extract2.png)

The easiest way to access the client is as follows:

- Navigate to the extracted files in windows explorer.
- in the URL bar type `CMD` and press enter

![image](https://user-images.githubusercontent.com/41549105/111911676-293d2800-8a2c-11eb-9471-d7f885b4f4c0.png)

This will open the Windows Command Prompt which looks like this:

![image](https://user-images.githubusercontent.com/41549105/116725994-ec0b7480-a99f-11eb-87be-3293d8857e04.png)

To start the client and create a new wallet use the following:

`Client.exe --wallet-file WALLET --create-wallet`

![image](https://user-images.githubusercontent.com/41549105/116726487-94213d80-a9a0-11eb-854b-7bd6e2cc14ba.png)

This will create a wallet file called `WALLET` in the same directory as the client.  

**NOTE** --create-wallet only needs to be passed when creating a new wallet.  When opening an existing wallet --create-wallet is not required.

![image](https://user-images.githubusercontent.com/41549105/116727247-89b37380-a9a1-11eb-9d76-640aebce875a.png)

This will start the CiviPort Client and connect to CiviSwarm and the bridge contracts. 

![image](https://user-images.githubusercontent.com/41549105/116727374-b5365e00-a9a1-11eb-9f76-c72774728da9.png)

Check your balances with `token-balance` for FMTA and other ERC-20's or `balance` for the Native chain's coin balances.

![image](https://user-images.githubusercontent.com/41549105/116767424-4a127900-a9ed-11eb-99d4-98ce39c1055b.png)

Starting an FMTA teleport is simple. To make a teleport of 10 FMTA from the Ethereum network to Binance Smart Chain using the `teleport` command enter:

`teleport 10 FMTA`

![image](https://user-images.githubusercontent.com/41549105/116767473-978ee600-a9ed-11eb-8482-e974e10a9eb9.png)

The client will ask for a source and destination network as well as get a gas estimate. It then asks permission to send and provides you with the Transaction ID (TX Passed) as well as Teleport ID once complete.  You can retrive all your wallets pending Teleport ID's by using the `pending` command.

![image](https://user-images.githubusercontent.com/41549105/116767619-885c6800-a9ee-11eb-96f7-f5f72420d1c6.png)

To complete the teleport we simply energize it using the `energize` command.

`energize 20b48c6022a68bb25bf760d954c7e67ff06dc85297356068c9fb3fd3e88991ec`

or alternatively just use `energize` and CiviPort will energize the last pending teleport. 

![image](https://user-images.githubusercontent.com/41549105/116767717-1e908e00-a9ef-11eb-8758-747eac4bf48d.png)

That's it!  You have succesfully sent Test FMTA from the Ethereum network to Binance Smart Chain!

### Linux and Mac

The above applies to Linux and mac operating systems but start the client using `./client --wallet-file WALLET --create-wallet` and your prefered method for unzipping.



