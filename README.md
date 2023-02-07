# CONCORDIUM_task_1
this is my submission for concordium hackaton event

## INSTALL RUST
# As im using vps so maybe the command will be different

- install Rust using [Rustup](https://rustup.rs/) using 
    ````
    curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
    ````
![Screenshot 2023-02-07 125053](https://user-images.githubusercontent.com/41656124/217164834-21614858-a676-479d-a514-afbd5f4073d1.png)

- install Wasm to using this command 
    ````
    rustup target add wasm32-unknown-unknown
    ````
    ![Screenshot 2023-02-07 125142](https://user-images.githubusercontent.com/41656124/217165139-2e321d19-4d58-4886-9816-a10b01f83081.png)

## INSTALL THE CARGO
since im using a vps im using wget
````
wget https://distribution.concordium.software/tools/linux/cargo-concordium_2.7.0
````
