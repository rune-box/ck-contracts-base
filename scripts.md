# Scripts

* [Code - Github](https://github.com/nervosnetwork/ckb-production-scripts/tree/master/c)
* Scripts - Nervos Explorer:
  * [Mainnet](https://explorer.nervos.org/scripts)
  * [Testnet](https://pudge.explorer.nervos.org/scripts)
---

* **Anyone-Can-Pay Lock**
  * anyone_can_pay allows a recipient to provide cell capacity in asset transfer.
  * Code Hash  
    * Mainnet: 0xd369597ff47f29fbc0d47d2e3775370d1250b85140c670e4718af712983a2354
    * Testnet: 0x3419a1c09eb2567f6552ee7a8ecffd64155cffe0f1796e6e61ec088d740c1356
  * [RFC](https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0026-anyone-can-pay/0026-anyone-can-pay.md)
  * Usage: TODO
* **CoTA**
  * A Compact Token Aggregator Standard for Extremely Low Cost NFTs and FTs.
  * Code Hash  
    * Mainnet: 0x1122a4fb54697cf2e6e3a96c9d80fd398a936559b90954c6e88eb7ba0cf652df
    * Testnet: 0x89cd8003a0eaf8e65e0c31525b7d1d5c1becefd2ea75bb4cff87810ae37764d8
  * Usage: TODO
* **CoTA Registry**
  * A Compact Token Aggregator Standard for Extremely Low Cost NFTs and FTs.
  * Code Hash  
    * Mainnet: 0x90ca618be6c15f5857d3cbd09f9f24ca6770af047ba9ee70989ec3b229419ac7
    * Testnet: 0x9302db6cc1344b81a5efee06962abcb40427ecfcbe69d471b01b2658ed948075
  * Usage: TODO
* **godwoken_challenge_lock**
  * When a Godwoken node found that an invalid state exists in the Rollup, the node can send the RollupEnterChallenge action to the Rollup cell and generate a challenging cell.
  * Code Hash  
    * Mainnet: 0x628b5f956b46ae27b50819a9ebab79ce5f957e6899ba0c75b8e142de2ed0dcd2
    * Testnet: 0x5a86c3bf1e8648b6a6f8abe6875720ccf9745ab225b68fa7c195f9d6635dea80
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/challenge-lock)
  * Usage: TODO
* **godwoken_custodian_lock**
  * Rollup uses the custodian lock to hold the deposited assets.
  * Code Hash  
    * Mainnet: 0x000f87062a2fe9bb4a6cc475212ea11014b84deb32e0375ee51e6ec4a553e009
    * Testnet: 0x85ae4db0dd83f428a31deb342e4000af37ce2c9645d9e619df00096e3c50a2bb
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/custodian-lock)
  * Usage: TODO
* **godwoken_deposit_lock**
  * A layer1 user can join the Rollup by creating a deposit cell.
  * Code Hash  
    * Mainnet: 0xff602581f07667eef54232cce850cbca2c418b3418611c132fca849d1edcd775
    * Testnet: 0x50704b84ecb4c4b12b43c7acb260ddd69171c21b4c0ba15f3c469b7d143f6f18
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/deposit-lock)
  * Usage: TODO
* **godwoken_eth_account_lock**
  * A layer-2 lock script, ETH account lock is a script that verifies the layer-2 account signature.
  * Code Hash  
    * Mainnet: 0x096df264f38fff07f3acd318995abc2c71ae0e504036fe32bc38d5b6037364d4
    * Testnet: 0x07521d0aa8e66ef441ebc31204d86bb23fc83e9edc58c19dbb1b0ebe64336ec0
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/eth-account-lock)
  * Usage: TODO
* **godwoken_stake_lock**
  * A block producer is required to provide a stake cell to perform the RollupSubmitBlock action.
  * Code Hash  
    * Mainnet: 0xb619184ab9142c51b0ee75f4e24bcec3d077eefe513115bad68836d06738fd2c
    * Testnet: 0x7f5a09b8bd0e85bcf2ccad96411ccba2f289748a1c16900b0635c2ed9126f288
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/stake-lock)
  * Usage: TODO
* **godwoken_state_validator**
  * State validator is the major script to verify the on-chain Rollup cell. Rollup cell is an identity cell on CKB, it stores the structure GlobalState which represents the layer-2 state.
  * Code Hash  
    * Mainnet: 0xfef1d086d9f74d143c60bf03bd04bab29200dbf484c801c72774f2056d4c6718
    * Testnet: 0x1e44736436b406f8e48a30dfbddcf044feb0c9eebfe63b0f81cb5bb727d84854
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/state-validator)
  * Usage: TODO
* **godwoken_withdrawal_lock**
  * Withdrawal cells are generated in the RollupSubmitBlock action according to the block.withdrawals field.
  * Code Hash  
    * Mainnet: 0x3714af858b8b82b2bb8f13d51f3cffede2dd8d352a6938334bb79e6b845e3658
    * Testnet: 0x06ae0706bb2d7997d66224741d3ec7c173dbb2854a6d2cf97088796b677269c6
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/withdrawal-lock)
  * Usage: TODO
* **m-NFT**
  * Code Hash  
    * Mainnet: 0x2b24f0d644ccbdd77bbf86b27c8cca02efa0ad051e447c212636d9ee7acaaec9
    * Testnet: 0xb1837b5ad01a88558731953062d1f5cb547adf89ece01e8934a9f0aeed2d959f
  * [RFC]()
  * Usage: TODO
* **Nervos DAO**
  * Nervos DAO is a smart contract with which users can interact the same way as any smart contract on CKB.
  * Code Hash  
    * Mainnet: 0x82d76d1b75fe2fd9a27dfbaa65a039221a380d76c926f378d3f81cf3e7e13f2e
    * Testnet: 0x82d76d1b75fe2fd9a27dfbaa65a039221a380d76c926f378d3f81cf3e7e13f2e
  * [RFC](https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0023-dao-deposit-withdraw/0023-dao-deposit-withdraw.md)
  * Usage: TODO
* **omni_lock v2**
  * Omnilock is a lock script designed for interoperability. It comes with built-in support for verification of transaction signing methods used in Bitcoin, Ethereum, EOS, and Dogecoin. Omnilock is also extensible, so more verification algorithms can be added in future.
  * Code Hash  
    * Mainnet: 0x9b819793a64463aed77c615d6cb226eea5487ccfc0783043a587254cda2b6f26
    * Testnet: 0xf329effd1c475a2978453c8600e1eaf0bc2087ee093c3ee64cc96ec6847752cb
  * [RFC](https://github.com/nervosnetwork/rfcs/tree/master/rfcs/0042-omnilock)
  * Usage: TODO
* **PW Lock (pwlock-k1-acpl)**
  * Forked from CKB's system scripts, and currently supports signature generated by personalSign and signTypedData from ethereum wallets.
  * Code Hash  
    * Mainnet: 0xbf43c3602455798c1a61a596e0d95278864c552fafe231c063b3fabf97a8febc
    * Testnet: 0x58c5f491aba6d61678b7cf7edf4910b1f5e00ec0cde2f42e0abb4fd9aff25a63
  * [Code](https://github.com/lay2dev/pw-lock/)
  * Usage: TODO
* **SECP256K1/blake160**
  * SECP256K1/blake160 is the default lock script to verify CKB transaction signature.
  * Code Hash  
    * Mainnet: 0x9bd7e06f3ecf4be0f2fcd2188b23f1b9fcc88e5d4b65a8637b17723bbda3cce8
    * Testnet: 0x9bd7e06f3ecf4be0f2fcd2188b23f1b9fcc88e5d4b65a8637b17723bbda3cce8
  * [RFC](https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0024-ckb-genesis-script-list/0024-ckb-genesis-script-list.md#secp256k1blake160)
  * Usage: TODO
* **SECP256K1/multisig**
  * SECP256K1/multisig is a script which allows a group of users to sign a single transaction.
  * Code Hash  
    * Mainnet: 0x5c5069eb0857efc65e1bca0c07df34c31663b3622fd3876c876320fc9634e2a8
    * Testnet: 0x5c5069eb0857efc65e1bca0c07df34c31663b3622fd3876c876320fc9634e2a8
  * [RFC](https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0024-ckb-genesis-script-list/0024-ckb-genesis-script-list.md#secp256k1multisig)
  * Usage: TODO
* **Simple UDT**
  * Simple UDT provides a way for dapp developers to issue custom tokens on Nervos CKB.
  * Code Hash  
    * Mainnet: 0x5e7a36a77e68eecc013dfa2fe6a23f3b6c344b04005808694ae6dd45eea4cfd5
    * Testnet: 0xc5e5dcf215925f7ef4dfaf5f4b4f105bc321c02776d6e7d52a1db3fcd9d011a4
  * [RFC](https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0025-simple-udt/0025-simple-udt.md)
  * Usage: TODO
* **UniPass v3**
  * UniPass Wallet is a smart contract wallet solution that supports on-chain Email social recovery.
  * Code Hash  
    * Mainnet: 0xd01f5152c267b7f33b9795140c2467742e8424e49ebe2331caec197f7281b60a
    * Testnet: 0x3e1eb7ed4809b2d60650be96a40abfbdafb3fb942b7b37ec7709e64e2cd0a783
  * Usage: TODO

