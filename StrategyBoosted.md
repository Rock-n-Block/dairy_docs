# StrategyBoosted









## Methods

### MAX_CALL_FEE

```solidity
function MAX_CALL_FEE() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### MAX_FEE

```solidity
function MAX_FEE() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### STRATEGIST_FEE

```solidity
function STRATEGIST_FEE() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### WITHDRAWAL_FEE_CAP

```solidity
function WITHDRAWAL_FEE_CAP() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### WITHDRAWAL_MAX

```solidity
function WITHDRAWAL_MAX() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### balanceOf

```solidity
function balanceOf() external view returns (uint256)
```



*calculate the total underlaying &#39;want&#39; held by the strat.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | total balance of DAIRY |

### balanceOfPool

```solidity
function balanceOfPool() external view returns (uint256)
```



*it calculates how much &#39;want&#39; the strategy has working in the farm.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | balance of DAIRY on staking contract |

### balanceOfWant

```solidity
function balanceOfWant() external view returns (uint256)
```



*it calculates how much &#39;want&#39; this contract holds.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | balance of DAIRY on this contract |

### beforeDeposit

```solidity
function beforeDeposit() external nonpayable
```



*call harvest before deposit if `harvestOnDeposit` is true*


### callFee

```solidity
function callFee() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### callReward

```solidity
function callReward() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | native reward amount for calling harvest |

### chef

```solidity
function chef() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | farm |

### dairyFee

```solidity
function dairyFee() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### dairyFeeRecipient

```solidity
function dairyFeeRecipient() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### deposit

```solidity
function deposit() external nonpayable
```



*puts the funds to work*


### gasprice

```solidity
function gasprice() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### getRPS

```solidity
function getRPS() external view returns (uint256)
```



*Method for APR/APY calculation*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | reward per second/block |

### harvest

```solidity
function harvest() external nonpayable
```



*call harvest*


### harvestOnDeposit

```solidity
function harvestOnDeposit() external view returns (bool)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | is `harvest()` calling on deposit |

### keeper

```solidity
function keeper() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### lastHarvest

```solidity
function lastHarvest() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | last harvest timestamp |

### lpToken0

```solidity
function lpToken0() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | token0 from pair |

### lpToken1

```solidity
function lpToken1() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | token1 from pair |

### managerHarvest

```solidity
function managerHarvest() external nonpayable
```

only manager available

*call harvest*


### native

```solidity
function native() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | WADA |

### output

```solidity
function output() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | MILKY |

### outputToLp0

```solidity
function outputToLp0() external view returns (address[])
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address[] | path for swap (MILKY-&gt;token0) |

### outputToLp0Route

```solidity
function outputToLp0Route(uint256) external view returns (address)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | MILKY -&gt; token0 |

### outputToLp1

```solidity
function outputToLp1() external view returns (address[])
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address[] | path for swap (MILKY-&gt;token1) |

### outputToLp1Route

```solidity
function outputToLp1Route(uint256) external view returns (address)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | MILKY -&gt; token1 |

### outputToNative

```solidity
function outputToNative() external view returns (address[])
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address[] | path for swap (MILKY-&gt;WADA) |

### outputToNativeRoute

```solidity
function outputToNativeRoute(uint256) external view returns (address)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | MILKY -&gt; WADA |

### owner

```solidity
function owner() external view returns (address)
```



*Returns the address of the current owner.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### panic

```solidity
function panic() external nonpayable
```

manager available only

*pauses deposits and withdraws all funds from third party systems.*


### pause

```solidity
function pause() external nonpayable
```

manager available only

*stop the contract and remove all allowances*


### paused

```solidity
function paused() external view returns (bool)
```



*Returns true if the contract is paused, and false otherwise.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### renounceOwnership

```solidity
function renounceOwnership() external nonpayable
```



*Leaves the contract without owner. It will not be possible to call `onlyOwner` functions anymore. Can only be called by the current owner. NOTE: Renouncing ownership will leave the contract without an owner, thereby removing any functionality that is only available to the owner.*


### retireStrat

```solidity
function retireStrat() external nonpayable
```

vault available only

*called as part of strat migration. Sends all the available funds back to the vault.*


### rewardsAvailable

```solidity
function rewardsAvailable() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | rewards unharvested |

### setCallFee

```solidity
function setCallFee(uint256 _fee) external nonpayable
```

manager available only

*change harvest call fee perc*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _fee | uint256 | new fee perc |

### setDairyFeeRecipient

```solidity
function setDairyFeeRecipient(address _dairyFeeRecipient) external nonpayable
```

owner available only

*Updates dairy fee recipient.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _dairyFeeRecipient | address | new dairy fee recipient address. |

### setHarvestOnDeposit

```solidity
function setHarvestOnDeposit(bool _harvestOnDeposit) external nonpayable
```

manager available only

*change status of `harvestOnDeposit`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _harvestOnDeposit | bool | new status |

### setKeeper

```solidity
function setKeeper(address _keeper) external nonpayable
```

manager available only

*Updates address of the strat keeper.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _keeper | address | new keeper address. |

### setShouldGasThrottle

```solidity
function setShouldGasThrottle(bool _shouldGasThrottle) external nonpayable
```

manager available only

*change status of `shouldGasThrottle`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _shouldGasThrottle | bool | new status |

### setStrategist

```solidity
function setStrategist(address _strategist) external nonpayable
```

current strategist available only

*Updates address where strategist fee earnings will go.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _strategist | address | new strategist address. |

### setUnirouter

```solidity
function setUnirouter(address _unirouter) external nonpayable
```

owner available only

*Updates router that will be used for swaps.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _unirouter | address | new unirouter address. |

### setVault

```solidity
function setVault(address _vault) external nonpayable
```

owner available only

*Updates parent vault.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _vault | address | new vault address. |

### setWithdrawalFee

```solidity
function setWithdrawalFee(uint256 _fee) external nonpayable
```

manager available only

*change withdrawal fee perc*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _fee | uint256 | new fee perc |

### shouldGasThrottle

```solidity
function shouldGasThrottle() external view returns (bool)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### strategist

```solidity
function strategist() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### transferOwnership

```solidity
function transferOwnership(address newOwner) external nonpayable
```



*Transfers ownership of the contract to a new account (`newOwner`). Can only be called by the current owner.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| newOwner | address | undefined |

### unirouter

```solidity
function unirouter() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### unpause

```solidity
function unpause() external nonpayable
```

manager available only

*start the contract and set all allowances*


### vault

```solidity
function vault() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### want

```solidity
function want() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | LP |

### withdraw

```solidity
function withdraw(uint256 _amount) external nonpayable
```

vault available only

*claim funds*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _amount | uint256 | value to claim |

### withdrawalFee

```solidity
function withdrawalFee() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |



## Events

### ChargedFees

```solidity
event ChargedFees(uint256 callFees, uint256 dairyFees, uint256 strategistFees)
```



*logs `chargeFees()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| callFees  | uint256 | call fee perc |
| dairyFees  | uint256 | dairy fee perc |
| strategistFees  | uint256 | strategist fee perc |

### Deposit

```solidity
event Deposit(uint256 tvl)
```



*logs `deposit()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| tvl  | uint256 | total staked amount |

### OwnershipTransferred

```solidity
event OwnershipTransferred(address indexed previousOwner, address indexed newOwner)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| previousOwner `indexed` | address | undefined |
| newOwner `indexed` | address | undefined |

### Paused

```solidity
event Paused(address account)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| account  | address | undefined |

### StratHarvest

```solidity
event StratHarvest(address indexed harvester, uint256 wantHarvested, uint256 tvl)
```



*logs `_harvest()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| harvester `indexed` | address | user address |
| wantHarvested  | uint256 | DAIRY claimed due to this harvest transaction |
| tvl  | uint256 | total staked amount |

### Unpaused

```solidity
event Unpaused(address account)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| account  | address | undefined |

### Withdraw

```solidity
event Withdraw(uint256 tvl)
```



*logs `withdraw()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| tvl  | uint256 | total staked amount |



