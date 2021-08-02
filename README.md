# Implementation of algorithms for solving the maximum flow problem
The following algorithms are implemented:<br/>
1. Push-relabel algorithm
1. Relabel-to-front algorithm

Example uses:

```python
from flow_network import FlowNetwork
from push_relabel import PushRelabel

network=FlowNetwork()

DS=[(0,2,10),(0,3,5),(2,3,15),(2,1,5),(3,1,10)]

network.loadNetworkFromDS(DS)

pr=PushRelabel(network,0,1)

print(pr.maxFlow())
```
