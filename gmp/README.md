# GMP

## Build and deploy a smart contract using Analog GMP interfaces on Sepolia 

### Build and Deploy

1. Открываем сайт https://remix.ethereum.org

2. Создаем новый файл [Counter.sol](https://github.com/madest92/analog-testnet/blob/main/gmp/Counter.sol)

3. Переходим во вкладку "Solidity compiler"

    1. Жмем **"Compile Counter.sol"**, использую версию компилятора 0.8.25

    ![plot](img/remixCreate.png)

4. Переходим в вкладку **"Deploy"**

    1. В поле Environment выбираем Metamask. (!) Обязательно проверьте, что в Metamask выбрана сеть Sepolia

    2. В поле **"adress gateway"** указываем **0x7702eD777B5d6259483baAD0FE8b9083eF937E2A** 

    3. Жмем **"Deploy"**, подтвержаем транзакцию. После копируем адрес контракта в **"Deployed/Unpinned Contracts"** внизу слева

    ![plot](img/remixDeploy.png)

### Verified

1. Открываем сайт https://eth-sepolia.blockscout.com/contract-verification

    * Вписываем адрес смарт контракта

    * Лицензия MIT

    * Метод верификации: Solidity(Flattened source code)

    * Версия компилятора: 0.8.25

    * Версия EVM: default

    * Убираем галочку с оптимизации

    * Вставляем тот же самый код из файла Counter.sol

    * Ждем Verify

![plot](./img/blockscout.png)

## Send a message using a GMP gateway contract

Пока не знаю....