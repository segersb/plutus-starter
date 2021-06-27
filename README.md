# Plutus Platform starter project

This project gives a simple starter project for using the Plutus Platform on Windows with VSCode.
The application is the Oracle from the Plutus Pioneer program lectures.

## Setting up

### WSL
This setup assumes you have configured WSL in Windows.

### VSCode
Open the project in WSL with Ubuntu as distro

Install the following packages in your WSL terminal
```sudo apt install pkg-confi```
```sudo apt install libsodium-dev```

Install the following VSCode extension
https://marketplace.visualstudio.com/items?itemName=haskell.haskell

### Running the code
1. Build the application by running ```cabal build```
2. Start the Plutus Application Backend app ```cabal run oralce-pab```
3. Wait until you see a ```oracle.cid``` file in your root directory
4. Start the oracle client app ```cabal run oralce-client```
5. Start the swap client apps ```cabal run swap-client -- 2``` ```cabal run swap-client -- 3```
