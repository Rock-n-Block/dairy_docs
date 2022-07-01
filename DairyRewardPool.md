# DairyRewardPool









## Methods

### DURATION

```solidity
function DURATION() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | day duration seconds value |

### balanceOf

```solidity
function balanceOf(address account) external view returns (uint256)
```



*total stake amount for current user*

#### Parameters

| Name | Type | Description |
|---|---|---|
| account | address | user address |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | user deposit balance |

### earned

```solidity
function earned(address account) external view returns (uint256)
```



*Get current reward for the user*

#### Parameters

| Name | Type | Description |
|---|---|---|
| account | address | user address |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | the current amount of rewards for the current user |

### exit

```solidity
function exit() external nonpayable
```



*Function for withdraw + getReward actions*


### getReward

```solidity
function getReward() external nonpayable
```



*Function for claim all rewards action*


### inCaseTokensGetStuck

```solidity
function inCaseTokensGetStuck(address _token) external nonpayable
```

available for an owner only

*Function for wrong tokens claiming*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _token | address | an address of wrong token to claim |

### lastTimeRewardApplicable

```solidity
function lastTimeRewardApplicable() external view returns (uint256)
```



*Get last timestamp of reward issue *


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | minimum between now and periodFinish variable |

### lastUpdateTime

```solidity
function lastUpdateTime() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | the last time of activity on the contract |

### notifyRewardAmount

```solidity
function notifyRewardAmount(uint256 reward) external nonpayable
```

available for an owner only (feeBatch)

*Function for reward adding*

#### Parameters

| Name | Type | Description |
|---|---|---|
| reward | uint256 | value of WETH to distribute |

### owner

```solidity
function owner() external view returns (address)
```



*Returns the address of the current owner.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### periodFinish

```solidity
function periodFinish() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | this variable means the end of the reward distribution period (when the reward is added on the contract, this variable is set to now() + 86400, i.e. plus a day. Means that the reward will be distributed every second evenly throughout the day) |

### renounceOwnership

```solidity
function renounceOwnership() external nonpayable
```



*Leaves the contract without owner. It will not be possible to call `onlyOwner` functions anymore. Can only be called by the current owner. NOTE: Renouncing ownership will leave the contract without an owner, thereby removing any functionality that is only available to the owner.*


### rewardPerToken

```solidity
function rewardPerToken() external view returns (uint256)
```



*Get current rate per 1 DAIRY*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | the current rate of the reward for the token (1 DAIRY) at the current moment |

### rewardPerTokenStored

```solidity
function rewardPerTokenStored() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | last saved rewardPerToken() (see `rewardPerToken()` func) |

### rewardRate

```solidity
function rewardRate() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | current rate (reward/86400; number of reward tokens released per second) |

### rewardToken

```solidity
function rewardToken() external view returns (contract IERC20)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | contract IERC20 | WETH address |

### rewards

```solidity
function rewards(address) external view returns (uint256)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | calculated saved rewards for the user |

### stake

```solidity
function stake(uint256 amount) external nonpayable
```

stake visibility is public as overriding LPTokenWrapper&#39;s stake() function

*Function for deposit action*

#### Parameters

| Name | Type | Description |
|---|---|---|
| amount | uint256 | value of deposit |

### stakedToken

```solidity
function stakedToken() external view returns (contract IERC20)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | contract IERC20 | undefined |

### totalSupply

```solidity
function totalSupply() external view returns (uint256)
```



*total stake amount*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | total deposit balance |

### transferOwnership

```solidity
function transferOwnership(address newOwner) external nonpayable
```



*Transfers ownership of the contract to a new account (`newOwner`). Can only be called by the current owner.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| newOwner | address | undefined |

### userRewardPerTokenPaid

```solidity
function userRewardPerTokenPaid(address) external view returns (uint256)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | `rewardPerTokenStored` for the current user |

### withdraw

```solidity
function withdraw(uint256 amount) external nonpayable
```

withdraw visibility is public as overriding LPTokenWrapper&#39;s withdraw() function

*Function for withdraw action*

#### Parameters

| Name | Type | Description |
|---|---|---|
| amount | uint256 | value of claim |



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

### RewardAdded

```solidity
event RewardAdded(uint256 reward)
```



*logs `notifyRewardAmount()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| reward  | uint256 | value of WETH for distribution |

### RewardPaid

```solidity
event RewardPaid(address indexed user, uint256 reward)
```



*logs `getReward()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| user `indexed` | address | user address |
| reward  | uint256 | value of reward claim |

### Staked

```solidity
event Staked(address indexed user, uint256 amount)
```



*logs `stake()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| user `indexed` | address | user address |
| amount  | uint256 | value of deposit |

### Withdrawn

```solidity
event Withdrawn(address indexed user, uint256 amount)
```



*logs `withdraw()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| user `indexed` | address | user address |
| amount  | uint256 | value of deposit claim |



