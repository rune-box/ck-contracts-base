# Scripts

## Reference
* [Code - Github](https://github.com/nervosnetwork/ckb-production-scripts/tree/master/c)
* Scripts - Nervos Explorer:
  * [Mainnet](https://explorer.nervos.org/scripts)
  * [Testnet](https://pudge.explorer.nervos.org/scripts)

---

* **Anyone-Can-Pay Lock**
  * anyone_can_pay allows a recipient to provide cell capacity in asset transfer.
  * Mainnet
  ```
  {
    "code_hash": "0xd369597ff47f29fbc0d47d2e3775370d1250b85140c670e4718af712983a2354",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x4153a2014952d7cac45f285ce9a7c5c0c0e1b21f2d378b82ac1433cb11c25c4d",
      "index": "0x0"
    },
    "dep_type": "dep_group"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x3419a1c09eb2567f6552ee7a8ecffd64155cffe0f1796e6e61ec088d740c1356",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xec26b0f85ed839ece5f11c4c4e837ec359f5adc4420410f6453b1f6b60fb96a6",
      "index": "0x0"
    },
    "dep_type": "dep_group"
  }
  ```
  * [RFC](https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0026-anyone-can-pay/0026-anyone-can-pay.md)
  * Usage: TODO
* **CoTA**
  * A Compact Token Aggregator Standard for Extremely Low Cost NFTs and FTs.
  * Mainnet
  ```
  {
    "code_hash": "0x1122a4fb54697cf2e6e3a96c9d80fd398a936559b90954c6e88eb7ba0cf652df",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x875db3381ebe7a730676c110e1c0d78ae1bdd0c11beacb7db4db08e368c2cd95",
      "index": "0x0"
    },
    "dep_type": "dep_group"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x89cd8003a0eaf8e65e0c31525b7d1d5c1becefd2ea75bb4cff87810ae37764d8",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xd8c7396f955348bd74a8ed4398d896dad931977b7c1e3f117649765cd3d75b86",
      "index": "0x0"
    },
    "dep_type": "dep_group"
  }
  ```
  * Usage: TODO
* **CoTA Registry**
  * A Compact Token Aggregator Standard for Extremely Low Cost NFTs and FTs.
  * Mainnet
  ```
  {
    "code_hash": "0x90ca618be6c15f5857d3cbd09f9f24ca6770af047ba9ee70989ec3b229419ac7",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x875db3381ebe7a730676c110e1c0d78ae1bdd0c11beacb7db4db08e368c2cd95",
      "index": "0x0"
    },
    "dep_type": "dep_group"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x9302db6cc1344b81a5efee06962abcb40427ecfcbe69d471b01b2658ed948075",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xd8c7396f955348bd74a8ed4398d896dad931977b7c1e3f117649765cd3d75b86",
      "index": "0x0"
    },
    "dep_type": "dep_group"
  }
  ```
  * Usage: TODO
* **godwoken_challenge_lock**
  * When a Godwoken node found that an invalid state exists in the Rollup, the node can send the RollupEnterChallenge action to the Rollup cell and generate a challenging cell.
  * Mainnet
  ```
  {
    "code_hash": "0x628b5f956b46ae27b50819a9ebab79ce5f957e6899ba0c75b8e142de2ed0dcd2",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x8eca99207a462a9005bd91d04e24911627769096220f867d1cc0a32e75a287a6",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x5a86c3bf1e8648b6a6f8abe6875720ccf9745ab225b68fa7c195f9d6635dea80",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x15598fb4d3fc4b7e0afcffc80ed0c02b62edb3f7875771f0397f17eef712b65d",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/challenge-lock)
  * Usage: TODO
* **godwoken_custodian_lock**
  * Rollup uses the custodian lock to hold the deposited assets.
  * Mainnet
  ```
  {
    "code_hash": "0x000f87062a2fe9bb4a6cc475212ea11014b84deb32e0375ee51e6ec4a553e009",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x71b55e3641fdc8d00d9943a93b2c6e6ab42f7e57909009c2a1ad5c234956cdc5",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x85ae4db0dd83f428a31deb342e4000af37ce2c9645d9e619df00096e3c50a2bb",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x7aed145beb6984fff008ca6224d0726d06a19959c4f01d15e49942d76e28747a",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/custodian-lock)
  * Usage: TODO
* **godwoken_deposit_lock**
  * A layer1 user can join the Rollup by creating a deposit cell.
  * Mainnet
  ```
  {
    "code_hash": "0xff602581f07667eef54232cce850cbca2c418b3418611c132fca849d1edcd775",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x61e576a7e5d2398ecc5b1a969d1af0142c87db0996c2f6fce41bf28f68d805b2",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x50704b84ecb4c4b12b43c7acb260ddd69171c21b4c0ba15f3c469b7d143f6f18",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x9caeec735f3cd2a60b9d12be59bb161f7c61ddab1ac22c4383a94c33ba6404a2",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/deposit-lock)
  * Usage: TODO
* **godwoken_eth_account_lock**
  * A layer-2 lock script, ETH account lock is a script that verifies the layer-2 account signature.
  * Mainnet
  ```
  {
    "code_hash": "0x096df264f38fff07f3acd318995abc2c71ae0e504036fe32bc38d5b6037364d4",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xf0cfb02fb435bf2f061cbf33b1b024a4944b3f4a95968a9d997d95dd2f76a7f9",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x07521d0aa8e66ef441ebc31204d86bb23fc83e9edc58c19dbb1b0ebe64336ec0",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x21da20f275af89ca7172cb1cd7fcb8676056e4212ba3782e8c77afebae57c6ed",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/eth-account-lock)
  * Usage: TODO
* **godwoken_stake_lock**
  * A block producer is required to provide a stake cell to perform the RollupSubmitBlock action.
  * Mainnet
  ```
  {
    "code_hash": "0xb619184ab9142c51b0ee75f4e24bcec3d077eefe513115bad68836d06738fd2c",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x2e46a10a67987594d4eaee2d5f9ac96ce651f7bfb44e82c286a12a1950ad4f29",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x7f5a09b8bd0e85bcf2ccad96411ccba2f289748a1c16900b0635c2ed9126f288",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x053fdb4ed3181eab3a3a5f05693b53a8cdec0a24569e16369f444bac48be7de9",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/stake-lock)
  * Usage: TODO
* **godwoken_state_validator**
  * State validator is the major script to verify the on-chain Rollup cell. Rollup cell is an identity cell on CKB, it stores the structure GlobalState which represents the layer-2 state.
  * Mainnet
  ```
  {
    "code_hash": "0xfef1d086d9f74d143c60bf03bd04bab29200dbf484c801c72774f2056d4c6718",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x9f8e73e096f1583696760281004d71dc0cebd3c9aa6fb584949facde6e543e67",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x1e44736436b406f8e48a30dfbddcf044feb0c9eebfe63b0f81cb5bb727d84854",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xbcd73881ba53f1cd95d0c855395c4ffe6f54e041765d9ab7602d48a7cb71612e",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/state-validator)
  * Usage: TODO
* **godwoken_withdrawal_lock**
  * Withdrawal cells are generated in the RollupSubmitBlock action according to the block.withdrawals field.
  * Mainnet
  ```
  {
    "code_hash": "0x3714af858b8b82b2bb8f13d51f3cffede2dd8d352a6938334bb79e6b845e3658",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xe6389b5cf63eec1e2592e930414bc43f92508e529bdd5f5a07fa1dd140f4f20a",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x06ae0706bb2d7997d66224741d3ec7c173dbb2854a6d2cf97088796b677269c6",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x9c607a9a75ea4699dd01b1c2a478002343998cac8346d2aa582f35b532bd2b93",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * [Code](https://github.com/godwokenrises/godwoken/tree/develop/gwos/contracts/withdrawal-lock)
  * Usage: TODO
* **m-NFT**
  * Mainnet
  ```
  {
    "code_hash": "0x2b24f0d644ccbdd77bbf86b27c8cca02efa0ad051e447c212636d9ee7acaaec9",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x5dce8acab1750d4790059f22284870216db086cb32ba118ee5e08b97dc21d471",
      "index": "0x2"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0xb1837b5ad01a88558731953062d1f5cb547adf89ece01e8934a9f0aeed2d959f",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xf11ccb6079c1a4b3d86abe2c574c5db8d2fd3505fdc1d5970b69b31864a4bd1c",
      "index": "0x2"
    },
    "dep_type": "code"
  }
  ```
  * [RFC]()
  * Usage: TODO
* **Nervos DAO**
  * Nervos DAO is a smart contract with which users can interact the same way as any smart contract on CKB.
  * Mainnet
  ```
  {
    "code_hash": "0x82d76d1b75fe2fd9a27dfbaa65a039221a380d76c926f378d3f81cf3e7e13f2e",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xe2fb199810d49a4d8beec56718ba2593b665db9d52299a0f9e6e75416d73ff5c",
      "index": "0x2"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x82d76d1b75fe2fd9a27dfbaa65a039221a380d76c926f378d3f81cf3e7e13f2e",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x8f8c79eb6671709633fe6a46de93c0fedc9c1b8a6527a18d3983879542635c9f",
      "index": "0x2"
    },
    "dep_type": "code"
  }
  ```
  * [RFC](https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0023-dao-deposit-withdraw/0023-dao-deposit-withdraw.md)
  * Usage: TODO
* **omni_lock v2**
  * Omnilock is a lock script designed for interoperability. It comes with built-in support for verification of transaction signing methods used in Bitcoin, Ethereum, EOS, and Dogecoin. Omnilock is also extensible, so more verification algorithms can be added in future.
  * Mainnet
  ```
  {
    "code_hash": "0x9b819793a64463aed77c615d6cb226eea5487ccfc0783043a587254cda2b6f26",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xdfdb40f5d229536915f2d5403c66047e162e25dedd70a79ef5164356e1facdc8",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0xf329effd1c475a2978453c8600e1eaf0bc2087ee093c3ee64cc96ec6847752cb",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x27b62d8be8ed80b9f56ee0fe41355becdb6f6a40aeba82d3900434f43b1c8b60",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * [RFC](https://github.com/nervosnetwork/rfcs/tree/master/rfcs/0042-omnilock)
  * Usage: TODO
* **PW Lock (pwlock-k1-acpl)**
  * Forked from CKB's system scripts, and currently supports signature generated by personalSign and signTypedData from ethereum wallets.
  * Mainnet
  ```
  {
    "code_hash": "0xbf43c3602455798c1a61a596e0d95278864c552fafe231c063b3fabf97a8febc",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x1d60cb8f4666e039f418ea94730b1a8c5aa0bf2f7781474406387462924d15d4",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x58c5f491aba6d61678b7cf7edf4910b1f5e00ec0cde2f42e0abb4fd9aff25a63",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x4f254814b972421789fafef49d4fee94116863138f72ab1e6392daf3decfaec1",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * [Code](https://github.com/lay2dev/pw-lock/)
  * Usage: TODO
* **SECP256K1/blake160**
  * SECP256K1/blake160 is the default lock script to verify CKB transaction signature.
  * Mainnet
  ```
  {
    "code_hash": "0x9bd7e06f3ecf4be0f2fcd2188b23f1b9fcc88e5d4b65a8637b17723bbda3cce8",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x71a7ba8fc96349fea0ed3a5c47992e3b4084b031a42264a018e0072e8172e46c",
      "index": "0x0"
    },
    "dep_type": "dep_group"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x9bd7e06f3ecf4be0f2fcd2188b23f1b9fcc88e5d4b65a8637b17723bbda3cce8",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xf8de3bb47d055cdf460d93a2a6e1b05f7432f9777c8c474abf4eec1d4aee5d37",
      "index": "0x0"
    },
    "dep_type": "dep_group"
  }
  ```
  * [RFC](https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0024-ckb-genesis-script-list/0024-ckb-genesis-script-list.md#secp256k1blake160)
  * Usage: TODO
* **SECP256K1/multisig**
  * SECP256K1/multisig is a script which allows a group of users to sign a single transaction.
  * Mainnet
  ```
  {
    "code_hash": "0x5c5069eb0857efc65e1bca0c07df34c31663b3622fd3876c876320fc9634e2a8",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x71a7ba8fc96349fea0ed3a5c47992e3b4084b031a42264a018e0072e8172e46c",
      "index": "0x1"
    },
    "dep_type": "dep_group"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x5c5069eb0857efc65e1bca0c07df34c31663b3622fd3876c876320fc9634e2a8",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xf8de3bb47d055cdf460d93a2a6e1b05f7432f9777c8c474abf4eec1d4aee5d37",
      "index": "0x1"
    },
    "dep_type": "dep_group"
  }
  ```
  * [RFC](https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0024-ckb-genesis-script-list/0024-ckb-genesis-script-list.md#secp256k1multisig)
  * Usage: TODO
* **Simple UDT**
  * Simple UDT provides a way for dapp developers to issue custom tokens on Nervos CKB.
  * Mainnet
  ```
  {
    "code_hash": "0x5e7a36a77e68eecc013dfa2fe6a23f3b6c344b04005808694ae6dd45eea4cfd5",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xc7813f6a415144643970c2e88e0bb6ca6a8edc5dd7c1022746f628284a9936d5",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0xc5e5dcf215925f7ef4dfaf5f4b4f105bc321c02776d6e7d52a1db3fcd9d011a4",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0xe12877ebd2c3c364dc46c5c992bcfaf4fee33fa13eebdf82c591fc9825aab769",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * [RFC](https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0025-simple-udt/0025-simple-udt.md)
  * Usage: TODO
* **UniPass v3**
  * UniPass Wallet is a smart contract wallet solution that supports on-chain Email social recovery.
  * Mainnet
  ```
  {
    "code_hash": "0xd01f5152c267b7f33b9795140c2467742e8424e49ebe2331caec197f7281b60a",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x86a5e91ad93475caf30a3d3b0258786dd463984f71e8471abc5574f206f6207a",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Testnet
  ```
  {
    "code_hash": "0x3e1eb7ed4809b2d60650be96a40abfbdafb3fb942b7b37ec7709e64e2cd0a783",
    "hash_type": "type",
    "out_point": {
      "tx_hash": "0x8b98ede6bf7b5baba767b1d2d46a13749fc810375b14152abbc259a7fc98e46d",
      "index": "0x0"
    },
    "dep_type": "code"
  }
  ```
  * Usage: TODO

