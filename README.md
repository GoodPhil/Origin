![배너 전환(0 7X3m)](https://github.com/user-attachments/assets/eda143b6-e44e-436c-bd07-057f6a2a4dc5)


## Origin 한국 유저를 위해 작성된 메뉴얼입니다.
###### DApp 에 접근 불가상황에 아래의 순서대로 따라하시면 언스테이킹이 가능합니다. 언스테이킹 권한 설정이 된 경우에 정상 작동합니다.
#


### 1. 스마트 컨트랙 도구 실행: [here](https://ethereum-smart-contract-interaction-tool.vercel.app).

![003](https://github.com/user-attachments/assets/ae01c495-e894-4027-b698-aa66ca5109b4)

#

### 2. 언스테이킹 실행을 위해 아래 코드창 오른쪽 버튼 <img width="38" alt="Copy" src="https://github.com/user-attachments/assets/3e2d6b1b-e0fd-4c5f-a8b7-644a13e38e67"/> 모양과 같은 아이콘 버튼 클릭하여 복사!!!




```
[
    {
      "inputs": [
        { "internalType": "address", "name": "_OHM", "type": "address" },
        { "internalType": "address", "name": "_sOHM", "type": "address" },
        { "internalType": "uint256", "name": "_epochLength", "type": "uint256" },
        { "internalType": "uint256", "name": "_firstEpochNumber", "type": "uint256" },
        { "internalType": "uint256", "name": "_firstEpochBlock", "type": "uint256" }
      ],
      "stateMutability": "nonpayable",
      "type": "constructor"
    },
    {
      "anonymous": false,
      "inputs": [
        { "indexed": true, "internalType": "address", "name": "previousOwner", "type": "address" },
        { "indexed": true, "internalType": "address", "name": "newOwner", "type": "address" }
      ],
      "name": "OwnershipPulled",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        { "indexed": true, "internalType": "address", "name": "previousOwner", "type": "address" },
        { "indexed": true, "internalType": "address", "name": "newOwner", "type": "address" }
      ],
      "name": "OwnershipPushed",
      "type": "event"
    },
    {
      "inputs": [],
      "name": "XPH",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [{ "internalType": "address", "name": "_recipient", "type": "address" }],
      "name": "claim",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "contractBalance",
      "outputs": [{ "internalType": "uint256", "name": "", "type": "uint256" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "distributor",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "epoch",
      "outputs": [
        { "internalType": "uint256", "name": "length", "type": "uint256" },
        { "internalType": "uint256", "name": "number", "type": "uint256" },
        { "internalType": "uint256", "name": "endBlock", "type": "uint256" },
        { "internalType": "uint256", "name": "distribute", "type": "uint256" }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    { "inputs": [], "name": "forfeit", "outputs": [], "stateMutability": "nonpayable", "type": "function" },
    {
      "inputs": [{ "internalType": "uint256", "name": "_amount", "type": "uint256" }],
      "name": "giveLockBonus",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "index",
      "outputs": [{ "internalType": "uint256", "name": "", "type": "uint256" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "locker",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "manager",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    { "inputs": [], "name": "pullManagement", "outputs": [], "stateMutability": "nonpayable", "type": "function" },
    {
      "inputs": [{ "internalType": "address", "name": "newOwner_", "type": "address" }],
      "name": "pushManagement",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    { "inputs": [], "name": "rebase", "outputs": [], "stateMutability": "nonpayable", "type": "function" },
    { "inputs": [], "name": "renounceManagement", "outputs": [], "stateMutability": "nonpayable", "type": "function" },
    {
      "inputs": [{ "internalType": "uint256", "name": "_amount", "type": "uint256" }],
      "name": "returnLockBonus",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "sXPH",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        { "internalType": "enum OlympusStaking.CONTRACTS", "name": "_contract", "type": "uint8" },
        { "internalType": "address", "name": "_address", "type": "address" }
      ],
      "name": "setContract",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [{ "internalType": "uint256", "name": "_warmupPeriod", "type": "uint256" }],
      "name": "setWarmup",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        { "internalType": "uint256", "name": "_amount", "type": "uint256" },
        { "internalType": "address", "name": "_recipient", "type": "address" }
      ],
      "name": "stake",
      "outputs": [{ "internalType": "bool", "name": "", "type": "bool" }],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    { "inputs": [], "name": "toggleDepositLock", "outputs": [], "stateMutability": "nonpayable", "type": "function" },
    {
      "inputs": [],
      "name": "totalBonus",
      "outputs": [{ "internalType": "uint256", "name": "", "type": "uint256" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        { "internalType": "uint256", "name": "_amount", "type": "uint256" },
        { "internalType": "bool", "name": "_trigger", "type": "bool" }
      ],
      "name": "unstake",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "warmupContract",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "name": "warmupInfo",
      "outputs": [
        { "internalType": "uint256", "name": "deposit", "type": "uint256" },
        { "internalType": "uint256", "name": "gons", "type": "uint256" },
        { "internalType": "uint256", "name": "expiry", "type": "uint256" },
        { "internalType": "bool", "name": "lock", "type": "bool" }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "warmupPeriod",
      "outputs": [{ "internalType": "uint256", "name": "", "type": "uint256" }],
      "stateMutability": "view",
      "type": "function"
    }
  ]
```



#

### 3. 스마트 컨트랙 도구 창과 사용자 본인의 디지털 웰렛 연결.

![002](https://github.com/user-attachments/assets/cbe334c5-7b48-460d-bf19-95676e94b9c3)


#

### 4. 스마트 컨트랙 도구 창의 `Paste ABI JSON here` 에 붙여넣기

![004](https://github.com/user-attachments/assets/137aec52-296c-486d-a884-4003b09f7f8c)



#

### 5. 스테이킹 주소 복사:
```
0x1964Ca90474b11FFD08af387b110ba6C96251Bfc
```


#

### 6. 스마트 컨트랙 도구 창의 `Contract Address` 에 붙여넣기

![005](https://github.com/user-attachments/assets/23dac6de-520f-46d4-938e-bf899db034d1)


#

### 7. Write Function: unstake

![006](https://github.com/user-attachments/assets/dbe494d7-acda-4935-8141-999ea529d0e1)



#

### 8. unstake 수량 입력.

![007](https://github.com/user-attachments/assets/5f44b071-9f58-425c-a993-a0695af6148c)


@ LGNS 수량 입력 예

| 0.1     | 1 | 12 | 123                       | 1,234                                               |
|----------|----------|------------|------------------------------|------------------------------------------------------------|
| 100000000 | 1000000000    | 12000000000      | 123000000000  | 1234000000000               |

 1개 부터는 0 을 9개 입력.
