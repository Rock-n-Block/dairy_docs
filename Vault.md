# Vault









## Methods

### allowance

```solidity
function allowance(address owner, address spender) external view returns (uint256)
```



*See {IERC20-allowance}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | undefined |
| spender | address | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### approve

```solidity
function approve(address spender, uint256 amount) external nonpayable returns (bool)
```



*See {IERC20-approve}. NOTE: If `amount` is the maximum `uint256`, the allowance is not updated on `transferFrom`. This is semantically equivalent to an infinite approval. Requirements: - `spender` cannot be the zero address.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| spender | address | undefined |
| amount | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### available

```solidity
function available() external view returns (uint256)
```



*Custom logic in here for how much the vault allows to be borrowed. We return 100% of tokens for now. Under certain conditions we might want to keep some of the system funds at hand in the vault, instead of putting them to work.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### balance

```solidity
function balance() external view returns (uint256)
```



*It calculates the total underlying value of {token} held by the system. It takes into account the vault contract balance, the strategy contract balance  and the balance deployed in other contracts as part of the strategy.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### balanceOf

```solidity
function balanceOf(address account) external view returns (uint256)
```



*See {IERC20-balanceOf}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| account | address | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### decimals

```solidity
function decimals() external view returns (uint8)
```



*Returns the number of decimals used to get its user representation. For example, if `decimals` equals `2`, a balance of `505` tokens should be displayed to a user as `5.05` (`505 / 10 ** 2`). Tokens usually opt for a value of 18, imitating the relationship between Ether and Wei. This is the value {ERC20} uses, unless this function is overridden; NOTE: This information is only used for _display_ purposes: it in no way affects any of the arithmetic of the contract, including {IERC20-balanceOf} and {IERC20-transfer}.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint8 | undefined |

### decreaseAllowance

```solidity
function decreaseAllowance(address spender, uint256 subtractedValue) external nonpayable returns (bool)
```



*Atomically decreases the allowance granted to `spender` by the caller. This is an alternative to {approve} that can be used as a mitigation for problems described in {IERC20-approve}. Emits an {Approval} event indicating the updated allowance. Requirements: - `spender` cannot be the zero address. - `spender` must have allowance for the caller of at least `subtractedValue`.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| spender | address | undefined |
| subtractedValue | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### deposit

```solidity
function deposit(uint256 _amount) external nonpayable
```



*The entrypoint of funds into the system. People deposit with this function into the vault. The vault is then in charge of sending funds into the strategy.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _amount | uint256 | undefined |

### depositAll

```solidity
function depositAll() external nonpayable
```



*A helper function to call deposit() with all the sender&#39;s funds.*


### earn

```solidity
function earn() external nonpayable
```



*Function to send funds into the strategy and put them to work. It&#39;s primarily called by the vault&#39;s deposit() function.*


### getPricePerFullShare

```solidity
function getPricePerFullShare() external view returns (uint256)
```



*Function for various UIs to display the current value of one of our yield tokens. Returns an uint256 with 18 decimals of how much underlying asset one vault share represents.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### inCaseTokensGetStuck

```solidity
function inCaseTokensGetStuck(address _token) external nonpayable
```

owner available only

*Rescues random funds stuck that the strat can&#39;t handle.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _token | address | address of the token to rescue. |

### increaseAllowance

```solidity
function increaseAllowance(address spender, uint256 addedValue) external nonpayable returns (bool)
```



*Atomically increases the allowance granted to `spender` by the caller. This is an alternative to {approve} that can be used as a mitigation for problems described in {IERC20-approve}. Emits an {Approval} event indicating the updated allowance. Requirements: - `spender` cannot be the zero address.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| spender | address | undefined |
| addedValue | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### name

```solidity
function name() external view returns (string)
```



*Returns the name of the token.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | string | undefined |

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


### strategy

```solidity
function strategy() external view returns (contract IStrategy)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | contract IStrategy | The strategy currently in use by the vault. |

### symbol

```solidity
function symbol() external view returns (string)
```



*Returns the symbol of the token, usually a shorter version of the name.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | string | undefined |

### totalSupply

```solidity
function totalSupply() external view returns (uint256)
```



*See {IERC20-totalSupply}.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### transfer

```solidity
function transfer(address to, uint256 amount) external nonpayable returns (bool)
```



*See {IERC20-transfer}. Requirements: - `to` cannot be the zero address. - the caller must have a balance of at least `amount`.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| to | address | undefined |
| amount | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### transferFrom

```solidity
function transferFrom(address from, address to, uint256 amount) external nonpayable returns (bool)
```



*See {IERC20-transferFrom}. Emits an {Approval} event indicating the updated allowance. This is not required by the EIP. See the note at the beginning of {ERC20}. NOTE: Does not update the allowance if the current allowance is the maximum `uint256`. Requirements: - `from` and `to` cannot be the zero address. - `from` must have a balance of at least `amount`. - the caller must have allowance for ``from``&#39;s tokens of at least `amount`.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | undefined |
| to | address | undefined |
| amount | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### transferOwnership

```solidity
function transferOwnership(address newOwner) external nonpayable
```



*Transfers ownership of the contract to a new account (`newOwner`). Can only be called by the current owner.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| newOwner | address | undefined |

### upgradeStrat

```solidity
function upgradeStrat(address _implementation) external nonpayable
```

owner available only

*It switches the active strat for the @param _implementation.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _implementation | address | undefined |

### want

```solidity
function want() external view returns (contract IERC20)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | contract IERC20 | DAIRY address |

### withdraw

```solidity
function withdraw(uint256 _shares) external nonpayable
```



*Function to exit the system. The vault will withdraw the required tokens from the strategy and pay up the token holder. A proportional number of IOU tokens are burned in the process.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _shares | uint256 | undefined |

### withdrawAll

```solidity
function withdrawAll() external nonpayable
```



*A helper function to call withdraw() with all the sender&#39;s funds.*




## Events

### Approval

```solidity
event Approval(address indexed owner, address indexed spender, uint256 value)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| owner `indexed` | address | undefined |
| spender `indexed` | address | undefined |
| value  | uint256 | undefined |

### OwnershipTransferred

```solidity
event OwnershipTransferred(address indexed previousOwner, address indexed newOwner)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| previousOwner `indexed` | address | undefined |
| newOwner `indexed` | address | undefined |

### Transfer

```solidity
event Transfer(address indexed from, address indexed to, uint256 value)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| from `indexed` | address | undefined |
| to `indexed` | address | undefined |
| value  | uint256 | undefined |

### UpgradeStrat

```solidity
event UpgradeStrat(address implementation)
```



*logs `upgradeStrat()`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| implementation  | address | address of new strategy |



