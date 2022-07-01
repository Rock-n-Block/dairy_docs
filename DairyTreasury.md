# DairyTreasury









## Methods

### owner

```solidity
function owner() external view returns (address)
```



*Returns the address of the current owner.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### renounceOwnership

```solidity
function renounceOwnership() external nonpayable
```



*Leaves the contract without owner. It will not be possible to call `onlyOwner` functions anymore. Can only be called by the current owner. NOTE: Renouncing ownership will leave the contract without an owner, thereby removing any functionality that is only available to the owner.*


### transferOwnership

```solidity
function transferOwnership(address newOwner) external nonpayable
```



*Transfers ownership of the contract to a new account (`newOwner`). Can only be called by the current owner.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| newOwner | address | undefined |

### withdrawBnb

```solidity
function withdrawBnb(address payable _to, uint256 _amount) external nonpayable
```

owner available only

*Claim native function*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _to | address payable | receiver address |
| _amount | uint256 | value to transer |

### withdrawTokens

```solidity
function withdrawTokens(address _token, address _to, uint256 _amount) external nonpayable
```

owner available only

*Claim tokens function*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _token | address | token address |
| _to | address | receiver address |
| _amount | uint256 | value to transer |



## Events

### OwnershipTransferred

```solidity
event OwnershipTransferred(address indexed previousOwner, address indexed newOwner)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| previousOwner `indexed` | address | undefined |
| newOwner `indexed` | address | undefined |



