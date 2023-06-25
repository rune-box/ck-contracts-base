# Common Contracts for Nervos CKB

> Yes, the repository name `Common Contracts Base` comes from `Common Knowledge Base`~ O(∩_∩)O

A Public Good focusing on multi-chain, which will demonstrate the cryptographic primitives on Nervos. This repository refactored and rewrote the logic from [rust-playground](https://github.com/rune-box/rust-playground) (PLAN), so if you wanna use the logic code of **DNA** in non-smart-contract environment, see [rust-playground](https://github.com/rune-box/rust-playground).

0. [start](start.md): The start of learning CKB development.
1. [scripts](scripts.md): The contracts scripts were organized from Nervos explorer.
2. contracts (TODO)
3. Code example of usage (TODO)

## Common Usage
> I still haven't tried a complete test.
> The test code come from [Testing part](https://docs.nervos.org/docs/labs/capsule-exec/).

0. Explanation
When deploy a contract, we can get `tx_hash` and `index`.  
Through `tx_hash` and `index`, we can call a deployed contract in another contract.

1. Deploy the `echo` contract and get `out_point` info.
```
let echo_bin = {
    let mut buf = Vec::new();
    File::open("../build/debug/echo")
        .unwrap()
        .read_to_end(&mut buf)
        .expect("read code");
    Bytes::from(buf)
};
let echo_out_point = context.deploy_cell(echo_bin);

// out_point has 2 properties:
//   tx_hash:H256
//   index: uint32.
```
2. Get `cell_dep` info by `out_point`.
```

let echo_dep = CellDep::new_builder()
    .out_point(echo_out_point)
    .build();

// cell dep:
//   dep_type: uint8. // 0=Code, 8=DepGroup
//   out_point
```

3. Reference the contract cell in transaction by `cell_dep`
```
// build transaction
let tx = TransactionBuilder::default()
    .input(input)
    .outputs(outputs)
    .outputs_data(outputs_data.pack())
    // reference to echo cell
    .cell_dep(echo_dep)
    .build();

```

4. Test
```
let err = context.verify_tx(&tx, MAX_CYCLES).unwrap_err();
// check the return code is 42
assert_script_error(err, 42);
```
