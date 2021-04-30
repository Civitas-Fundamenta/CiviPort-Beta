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

![image](https://user-images.githubusercontent.com/41549105/111911826-a8326080-8a2c-11eb-82d0-bacdf112f773.png)

To start the client and create a new wallet use the following:

`Client.exe --testnet --wallet-file WALLET --create-wallet`

![image](https://user-images.githubusercontent.com/41549105/111911980-445c6780-8a2d-11eb-9993-b97c14d2d422.png)

This will create a wallet file called `WALLET` in the same directory as the client.  

**NOTE** --create-wallet only needs to be passed when creating a new wallet.  When opening an existing wallet --create-wallet is not required.

![image](https://user-images.githubusercontent.com/41549105/111912044-808fc800-8a2d-11eb-96a8-7c4f2ceecd9f.png)

This will start the CiviPort Client and connect to CiviSwarm and the bridge contracts. 

![image](https://user-images.githubusercontent.com/41549105/111912034-7077e880-8a2d-11eb-9512-acc8d7e03098.png)

To take part in testing you will need to have Test FMTA as well as SPOA and kETH from the solol and kovan testnets.  To get your wallets address simply type the command `address`.  Please come to https://t.me/CivitasFundamenta and paste your address to recieve test FMTA.  

To get Testnet coins for the native chains use the following faucets:

https://gitter.im/kovan-testnet/faucet# (You require a Twitter or Github account for this)

https://faucet-sokol.herokuapp.com/

https://faucet.matic.network/

https://faucet.goerli.mudit.blog/ (Requires Twitter)

https://faucet.rinkeby.io/ (Requires Twitter)

https://testnet.binance.org/faucet-smart (Requires Twitter)

Once you have the required coins testing can begin!

Check your balances with `fmta-balance` for FMTA or `balance` for the Native chain's coin balances.

![image](https://user-images.githubusercontent.com/41549105/111928595-b064bd00-8a79-11eb-907e-84dc41d5b157.png)

Starting an FMTA teleport is simple. To make a teleport of 10 FMTA from the Kovan to Sokol Testnet Using the `teleport` command enter:

`teleport 10 kovan sokol`

![image](https://user-images.githubusercontent.com/41549105/111928909-9e374e80-8a7a-11eb-8477-a1a5b5299776.png)

The client will get a gas estimate and ask permission to send and then provide you with the Transaction ID (TX Passed) as well as Teleport ID.  The Teleport ID will be required to complete the teleport.  You can retrive all your wallets pending Teleport ID's by using the `pending` command.

![image](https://user-images.githubusercontent.com/41549105/111929096-0a19b700-8a7b-11eb-9101-06b91e309dac.png)

To complete the teleport we simply energize it using the `energize` command.

`energize e7f057609ddbba6176c6924fef9712f1c51b595e09cd24f607115a3c0b342256`

![image](https://user-images.githubusercontent.com/41549105/111929192-43eabd80-8a7b-11eb-912a-132a9a1c50db.png)

That's it!  You have succesfully sent Test FMTA from the Kovan to Sokol Testnet!

### Linux and Mac

The above applies to Linux and mac operating systems but start the client using `./client --testnet --wallet-file WALLET --create-wallet` and your prefered method for unzipping.



