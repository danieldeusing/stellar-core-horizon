## Stellar Core Horizon  

### The simplest and cleanest Docker image for running stellar core and horizon

Build and run:
```
docker-compose build
docker-compose up -d
```

Creates a folder 'stellar' in your home folder.  Everything is stored there, delete it to reset.

This docker downloads and uses executables for core and horizon from Stellar.
If you want to build from stellars master branch on GitHub, Find BUILD_FROM_SRC and set to 1.
Find BUILD_FROM_SRC in /core-docker/Dockerfile and horizon-docker/Dockerfile

SSL NOTE:
Start it up once and stop it, for SSL to work you need to copy a folder named 'tsl' inside ~/stellar/node/horizon with your server.crt and server.key

Defaults to testnet.

Edit docker-compose.yml for mainnet

Pull requests welcome!
