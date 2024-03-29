# CONCORDIUM_task_1
THIS IS MY SUBMISSION FOR CONCORDIUM TASK 1

- My Mainnet Concordium wallet : 3fZro3wkcwmDLUUmqPiPfmCHwP68sHBaiaMREbQieSZ5eqvBZf
- ERC20 address : 0x85Dd8B04c87813e05dE105320E4fA661e8d3813C


## INSTALL RUST
# Since im using vps so maybe the command will be different

- install Rust [Rustup](https://rustup.rs/) using 
    ````
    curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
    ````
    ![Screenshot 2023-02-07 125053](https://user-images.githubusercontent.com/41656124/217164834-21614858-a676-479d-a514-afbd5f4073d1.png)

- install the Wasm using this command 
    ````
    rustup target add wasm32-unknown-unknown
    ````
    ![Screenshot 2023-02-07 125142](https://user-images.githubusercontent.com/41656124/217165139-2e321d19-4d58-4886-9816-a10b01f83081.png)

## Install the Concordium Cargo
- since im using a vps im using wget
    ````
    wget https://distribution.concordium.software/tools/linux/cargo-concordium_2.7.0
    ````
    ![Screenshot 2023-02-07 131014](https://user-images.githubusercontent.com/41656124/217166750-8f1f461d-1a8b-48ca-8a9d-5cc2717d5b7d.png)

- rename the file,make it executable and move it to system path,and check the version
    ````
    mv cargo-concordium_2.7.0 cargo-concordium
    chmod +x cargo-concordium
    sudo mv cargo-concordium /usr/local/bin
    cargo-concordium --version
    ````
    ![rename and make it excutable](https://user-images.githubusercontent.com/41656124/217166884-2db42dc2-0472-4888-8f59-64fe8b026bff.png)

- make sure its installed properly with
    ````
    cargo concordium --help
    ````
    ![the result of --help](https://user-images.githubusercontent.com/41656124/217167442-9296d483-af3b-473c-adb4-a58c473c19c9.png)

## Install Concordium Client
- download the client
    ````
    wget https://distribution.concordium.software/tools/linux/concordium-client_5.0.2-0
    ````
    ![download client on a server](https://user-images.githubusercontent.com/41656124/217167930-afe098b7-d046-4218-afd1-7071c8c3d5e4.png)

- rename the file,make it executable and move it to system path,and check the version
    ````
    mv concordium-client_5.0.2-0 concordium-client
    chmod +x concordium-client
    sudo mv concordium-client /usr/local/bin
    ````
- check if its intalled properly
    ````
    concordium-client --help
    ````
    ![rename client and moving to usr and check wheter its intalled properly](https://user-images.githubusercontent.com/41656124/217168621-121efa79-143b-4aae-bf3e-e383bd3b14e5.png)

## Install Web Wallet
- install [chrome extension](https://chrome.google.com/webstore/detail/concordium-wallet/mnnkpffndmickbiakofclnpoiajlegmg?hl=en-US)

![image](https://user-images.githubusercontent.com/41656124/217176954-cc3827a0-1f07-4e79-95e3-3b50c4754c0f.png)


## Creating Testnet Account
- creating ID using Concordium testnet IP (just create it, you can edit later)


  ![image](https://user-images.githubusercontent.com/41656124/217169515-7fe2cbc2-76d8-4fdb-b563-d516321dedcb.png)
  ![image](https://user-images.githubusercontent.com/41656124/217169601-3adf5b07-fe3c-4af8-9c9e-e20c668fb0f9.png)
  
 
- create an account

![image](https://user-images.githubusercontent.com/41656124/217170073-f919f1a6-f7aa-4524-a884-d974dc54d567.png)

- and request the testnet token (click on the blue circle)

![image](https://user-images.githubusercontent.com/41656124/217170530-e2ca6a54-5c6f-4eeb-8809-0a8906b4f419.png)

 ## Export The Key
- export your private key using setting in the extension -> export private key
- drag and drop the file to the vps

    ![image](https://user-images.githubusercontent.com/41656124/217171414-ad9e8245-9fe9-480a-b0c2-236ce024feb1.png)

- run  
    ````
    concordium-client config account import <YOUR PUBLIC ADDRESS.export> --name <Your-Wallet-Name> 
    ````
    the output should be like this
    ![image](https://user-images.githubusercontent.com/41656124/217171624-57334ee6-e76b-409a-a2d4-cd0ba3d5e7d7.png)

   



