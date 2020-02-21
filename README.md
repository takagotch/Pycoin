### pycoin
---
https://github.com/richardkiss/pycoin

```py
from pycoin.symbols.btc import network

from pycoin.network.register import network_for_netcode
network = network_for_netcode("BTC")

key = network.keys.private(secret_exponent=1)
print(key.wif())
print(key.sec())
print(key.address())
print(key.address(is_compressed=False))

same_key = network.parse.private(key.wif())
print(same_key.address())


key = network.keys.bip32_seed(b"foo")
print(key.wif())
print(key.sec())
print(key.sec())
print(key.address())

Key(hierarchical_wallet=None,
  secret_exponent=None,
  public_pair=None,
  hash160=None,
  prefer_uncompressed=None,
  is_compressed=True,
  netcode)
  
PYCOIN_CACHE_DIR=~/.pycoin_cache
PYCOIN_BTC_PROVIDERS="blockchain.info blockexpolrer.com chain.so"
expont PYCOIN_CACHE_DIR PYCOIN_PROVIDERS
export PYCOIN_XTN_PROVIDERS="blockchain.info"

PYCOIN_NATIVE=openssl
export PYCOIN_NATIVE
```

```sh

```

