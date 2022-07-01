# DairyFeeBatchV2









## Methods

### MAX_FEE

```solidity
function MAX_FEE() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | 100%, denominator |

### diary

```solidity
function diary() external view returns (contract IERC20Upgradeable)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | contract IERC20Upgradeable | DIARY address |

### harvest

```solidity
function harvest() external nonpayable
```



*Main function. Divides Diary&#39;s profits.*


### inCaseTokensGetStuck

```solidity
function inCaseTokensGetStuck(address _token, address _recipient) external nonpayable
```

owner available only

*Rescue locked funds sent by mistake*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _token | address | address of stuck token |
| _recipient | address | to |

### initRouter

```solidity
function initRouter(address _unirouter) external nonpayable
```

owner available only

*Manage the contract: set new router address (first time)*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _unirouter | address | new router |

### initialize

```solidity
function initialize(address _diary, address _wNative, address _treasury, address _rewardPool, address _unirouter) external nonpayable
```

initializer available only

*Initialize function for variables setting*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _diary | address | DIARY address |
| _wNative | address | WETH address |
| _treasury | address | treasury address |
| _rewardPool | address | staking address |
| _unirouter | address | router address |

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


### rewardPool

```solidity
function rewardPool() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | staking pool address |

### rewardPoolFee

```solidity
function rewardPoolFee() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | percent for staking pool fee distribution |

### routerInitialized

```solidity
function routerInitialized() external view returns (bool)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | is `unirouter` non zero |

### setNativeToDiaryRoute

```solidity
function setNativeToDiaryRoute(address[] _route) external nonpayable
```

owner available only

*Manage the contract: set new path*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _route | address[] | new path |

### setRewardPool

```solidity
function setRewardPool(address _rewardPool) external nonpayable
```

owner available only

*Manage the contract: set new staking address*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _rewardPool | address | new staking |

### setTreasury

```solidity
function setTreasury(address _treasury) external nonpayable
```

owner available only

*Manage the contract: set new treasury address*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _treasury | address | new treasury |

### setTreasuryFee

```solidity
function setTreasuryFee(uint256 _fee) external nonpayable
```

owner available only

*Manage the contract: set new treasury fee percent*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _fee | uint256 | new fee percent |

### setUnirouter

```solidity
function setUnirouter(address _unirouter) external nonpayable
```

owner available only

*Manage the contract: set new router address*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _unirouter | address | new router |

### transferOwnership

```solidity
function transferOwnership(address newOwner) external nonpayable
```



*Transfers ownership of the contract to a new account (`newOwner`). Can only be called by the current owner.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| newOwner | address | undefined |

### transferRewardPoolOwnership

```solidity
function transferRewardPoolOwnership(address _newOwner) external nonpayable
```

owner available only

*Function to change the staking&#39;s owner address (from this contract to an account)*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _newOwner | address | address of new owner |

### treasury

```solidity
function treasury() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | treasury address |

### treasuryFee

```solidity
function treasuryFee() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | percent for treasury fee distribution |

### unirouter

```solidity
function unirouter() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | router address |

### wNative

```solidity
function wNative() external view returns (contract IERC20Upgradeable)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | contract IERC20Upgradeable | WETH address |

### wNativeToDiaryRoute

```solidity
function wNativeToDiaryRoute(uint256) external view returns (address)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | path for swap (WETH -&gt; DIARY) |



## Events

### Initialized

```solidity
event Initialized(uint8 version)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| version  | uint8 | undefined |

### NewDiaryRoute

```solidity
event NewDiaryRoute(address[] oldRoute, address[] newRoute)
```



*logs `setNativeToDiaryRoute()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| oldRoute  | address[] | old path address |
| newRoute  | address[] | new path address |

### NewRewardPool

```solidity
event NewRewardPool(address oldRewardPool, address newRewardPool)
```



*logs `setRewardPool()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| oldRewardPool  | address | old staking address |
| newRewardPool  | address | new staking address |

### NewTreasury

```solidity
event NewTreasury(address oldTreasury, address newTreasury)
```



*logs `setTreasury()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| oldTreasury  | address | old treasury address |
| newTreasury  | address | new treasury address |

### NewUnirouter

```solidity
event NewUnirouter(address oldUnirouter, address newUnirouter)
```



*logs `setUnirouter()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| oldUnirouter  | address | old router address |
| newUnirouter  | address | new router address |

### OwnershipTransferred

```solidity
event OwnershipTransferred(address indexed previousOwner, address indexed newOwner)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| previousOwner `indexed` | address | undefined |
| newOwner `indexed` | address | undefined |



