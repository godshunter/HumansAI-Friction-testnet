# Hi!

## Restart 1 2023-05-15 21:37:02 CEST. --
~~~bash sudo systemctl restart humansd && sudo journalctl -u humansd -f
-- Logs begin at Mon 2023-05-15 21:37:02 CEST. --
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[2471517]: 4:22PM INF service stop impl={"Logger":{},"Switch":{"Logger":{}}} module=pex msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[2471517]: 4:22PM INF service stop book=/root/.humansd/config/addrbook.json impl={"Logger":{}} module=p2p msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[2471517]: 4:22PM ERR Stopped accept routine, as transport is closed module=p2p numPeers=0 server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[2471517]: 4:22PM INF Closing rpc listener listener={"Listener":{}} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[2471517]: 4:22PM INF Saving AddrBook to file book=/root/.humansd/config/addrbook.json module=p2p server=node size=121
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[2471517]: 4:22PM INF RPC HTTP server stopped err="accept tcp [::]:26657: use of closed network connection" module=rpc-server server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[2471517]: 4:22PM ERR Error serving server err="accept tcp [::]:26657: use of closed network connection" server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal systemd[1]: humansd.service: Succeeded.
May 19 16:22:55 Ubuntu-2004-focal-64-minimal systemd[1]: Stopped Humans node.
May 19 16:22:55 Ubuntu-2004-focal-64-minimal systemd[1]: Started Humans node.
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Unlocking keyring
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF starting ABCI with Tendermint
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF starting node with ABCI Tendermint in-process
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=multiAppConn module=proxy msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start connection=query impl=localClient module=abci-client msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start connection=snapshot impl=localClient module=abci-client msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start connection=mempool impl=localClient module=abci-client msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start connection=consensus impl=localClient module=abci-client msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=EventBus module=events msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=PubSub module=pubsub msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=IndexerService module=txindex msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF ABCI Handshake App Info hash="\u0087�O\x1aq\x14�ݪ\x18��S�s\x14�\x17�j�ڝ�J��߶`\b" height=115245 module=consensus protocol-version=0 server=node software-version=0.2.2
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF ABCI Replay Blocks appHeight=115245 module=consensus server=node stateHeight=115245 storeHeight=115245
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Completed ABCI Handshake - CometBFT and App are synced appHash="\u0087�O\x1aq\x14�ݪ\x18��S�s\x14�\x17�j�ڝ�J��߶`\b" appHeight=115245 module=consensus server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Version info abci=0.17.0 block=11 cmtbft_version=0.34.27 commit_hash= p2p=8 server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF This node is a validator addr=A5AD742A8FB77530A69CC9B772D7D2610CA29907 module=consensus pubKey=uhkgaTMe+rHTTB8fV76uLJCI4AEPj55WjnmJgy17mDU= server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF P2P Node ID ID=df5cb643d8aeade8ef288a3dd90e4fd8220954ba file=/root/.humansd/config/node_key.json module=p2p server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Adding persistent peers addrs=[] module=p2p server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Adding unconditional peer ids ids=[] module=p2p server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Add our address to book addr={"id":"df5cb643d8aeade8ef288a3dd90e4fd8220954ba","ip":"0.0.0.0","port":36656} book=/root/.humansd/config/addrbook.json module=p2p server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Add our address to book addr={"id":"df5cb643d8aeade8ef288a3dd90e4fd8220954ba","ip":"0.0.0.0","port":36656} book=/root/.humansd/config/addrbook.json module=p2p server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=Node msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Starting pprof server laddr=localhost:6061 server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl="P2P Switch" module=p2p msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF serve module=rpc-server msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=BlockchainReactor module=blockchain msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=BlockPool module=blockchain msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=ConsensusReactor module=consensus msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Reactor  module=consensus server=node waitSync=true
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=Evidence module=evidence msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=StateSync module=statesync msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=PEX module=pex msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start book=/root/.humansd/config/addrbook.json impl=AddrBook module=p2p msg={} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Saving AddrBook to file book=/root/.humansd/config/addrbook.json module=p2p server=node size=121
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Ensure peers module=pex numDialing=0 numInPeers=0 numOutPeers=0 numToDial=10 server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl="Peer{MConn{136.243.136.241:26656} 946b549550e9c564193bf4c963d84b17e5415a50 out}" module=p2p msg={} peer={"id":"946b549550e9c564193bf4c963d84b17e5415a50","ip":"136.243.136.241","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=MConn{136.243.136.241:26656} module=p2p msg={} peer={"id":"946b549550e9c564193bf4c963d84b17e5415a50","ip":"136.243.136.241","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl="Peer{MConn{94.237.27.19:26656} 42f95015c31c7814b6a0a717fd8c63d15f896e88 out}" module=p2p msg={} peer={"id":"42f95015c31c7814b6a0a717fd8c63d15f896e88","ip":"94.237.27.19","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=MConn{94.237.27.19:26656} module=p2p msg={} peer={"id":"42f95015c31c7814b6a0a717fd8c63d15f896e88","ip":"94.237.27.19","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl="Peer{MConn{178.23.126.70:26656} fa9eb901a01430d928e71162151992c7afb51d62 out}" module=p2p msg={} peer={"id":"fa9eb901a01430d928e71162151992c7afb51d62","ip":"178.23.126.70","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=MConn{178.23.126.70:26656} module=p2p msg={} peer={"id":"fa9eb901a01430d928e71162151992c7afb51d62","ip":"178.23.126.70","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl="Peer{MConn{135.181.142.117:26656} 459bcaea161d20cddcdead811d282bd495446cbb out}" module=p2p msg={} peer={"id":"459bcaea161d20cddcdead811d282bd495446cbb","ip":"135.181.142.117","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=MConn{135.181.142.117:26656} module=p2p msg={} peer={"id":"459bcaea161d20cddcdead811d282bd495446cbb","ip":"135.181.142.117","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl="Peer{MConn{95.217.200.36:26656} 2f6cc8b0b255745d71c358351ddde1faa350b0be out}" module=p2p msg={} peer={"id":"2f6cc8b0b255745d71c358351ddde1faa350b0be","ip":"95.217.200.36","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=MConn{95.217.200.36:26656} module=p2p msg={} peer={"id":"2f6cc8b0b255745d71c358351ddde1faa350b0be","ip":"95.217.200.36","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF starting API server... server=api
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF serve msg={} server=api
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl="Peer{MConn{38.146.3.209:26656} 6c2581bce457207a8d29895216a06f0f98d39599 out}" module=p2p msg={} peer={"id":"6c2581bce457207a8d29895216a06f0f98d39599","ip":"38.146.3.209","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=MConn{38.146.3.209:26656} module=p2p msg={} peer={"id":"6c2581bce457207a8d29895216a06f0f98d39599","ip":"38.146.3.209","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl="Peer{MConn{142.165.207.19:36656} 4762fa22edb91acd78010026f8da5fb71e174acb out}" module=p2p msg={} peer={"id":"4762fa22edb91acd78010026f8da5fb71e174acb","ip":"142.165.207.19","port":36656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=MConn{142.165.207.19:36656} module=p2p msg={} peer={"id":"4762fa22edb91acd78010026f8da5fb71e174acb","ip":"142.165.207.19","port":36656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl="Peer{MConn{206.125.33.0:26656} d7eb0e65cecbeeaa649b0a2fdf95ca2fb9f0cc3e out}" module=p2p msg={} peer={"id":"d7eb0e65cecbeeaa649b0a2fdf95ca2fb9f0cc3e","ip":"206.125.33.0","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=MConn{206.125.33.0:26656} module=p2p msg={} peer={"id":"d7eb0e65cecbeeaa649b0a2fdf95ca2fb9f0cc3e","ip":"206.125.33.0","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl="Peer{MConn{143.110.190.223:26656} 5ca0389db000da1ce87d992816a4aefa387c3998 out}" module=p2p msg={} peer={"id":"5ca0389db000da1ce87d992816a4aefa387c3998","ip":"143.110.190.223","port":26656} server=node
May 19 16:22:55 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=MConn{143.110.190.223:26656} module=p2p msg={} peer={"id":"5ca0389db000da1ce87d992816a4aefa387c3998","ip":"143.110.190.223","port":26656} server=node
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Time to switch to consensus reactor! height=115246 module=blockchain server=node
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service stop impl={"Logger":{}} module=blockchain msg={} server=node
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF SwitchToConsensus module=consensus server=node
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=ConsensusState module=consensus msg={} server=node
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=baseWAL module=consensus msg={} server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=Group module=consensus msg={} server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF service start impl=TimeoutTicker module=consensus msg={} server=node
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Searching for height height=115246 max=5686 min=5589 module=consensus server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Searching for height height=115245 max=5686 min=5589 module=consensus server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Found height=115245 index=5686 module=consensus server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Catchup by replaying consensus messages height=115246 module=consensus server=node
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Replay: New Step height=115246 module=consensus round=0 server=node step=RoundStepNewHeight
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Replay: Vote blockID={"hash":"06C846E8FD8D3736293BECDD17B51F6DED41B5E02792FDC193EFB251AB47CDCC","parts":{"hash":"07F449C5460D97F2B599A242F59235293A74A569A34C0369E11C360699A80DCA","total":1}} height=115245 module=consensus peer=8855d5696c4aec427051bd2ed3262e7e3a37f34d round=0 server=node type=2
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Replay: Vote blockID={"hash":"06C846E8FD8D3736293BECDD17B51F6DED41B5E02792FDC193EFB251AB47CDCC","parts":{"hash":"07F449C5460D97F2B599A242F59235293A74A569A34C0369E11C360699A80DCA","total":1}} height=115245 module=consensus peer=8855d5696c4aec427051bd2ed3262e7e3a37f34d round=0 server=node type=2
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Replay: Vote blockID={"hash":"06C846E8FD8D3736293BECDD17B51F6DED41B5E02792FDC193EFB251AB47CDCC","parts":{"hash":"07F449C5460D97F2B599A242F59235293A74A569A34C0369E11C360699A80DCA","total":1}} height=115245 module=consensus peer=8855d5696c4aec427051bd2ed3262e7e3a37f34d round=0 server=node type=2
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Replay: Vote blockID={"hash":"06C846E8FD8D3736293BECDD17B51F6DED41B5E02792FDC193EFB251AB47CDCC","parts":{"hash":"07F449C5460D97F2B599A242F59235293A74A569A34C0369E11C360699A80DCA","total":1}} height=115245 module=consensus peer=8855d5696c4aec427051bd2ed3262e7e3a37f34d round=0 server=node type=2
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Replay: Vote blockID={"hash":"06C846E8FD8D3736293BECDD17B51F6DED41B5E02792FDC193EFB251AB47CDCC","parts":{"hash":"07F449C5460D97F2B599A242F59235293A74A569A34C0369E11C360699A80DCA","total":1}} height=115245 module=consensus peer=8855d5696c4aec427051bd2ed3262e7e3a37f34d round=0 server=node type=2
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Replay: Vote blockID={"hash":"06C846E8FD8D3736293BECDD17B51F6DED41B5E02792FDC193EFB251AB47CDCC","parts":{"hash":"07F449C5460D97F2B599A242F59235293A74A569A34C0369E11C360699A80DCA","total":1}} height=115245 module=consensus peer=8855d5696c4aec427051bd2ed3262e7e3a37f34d round=0 server=node type=2
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Replay: Vote blockID={"hash":"06C846E8FD8D3736293BECDD17B51F6DED41B5E02792FDC193EFB251AB47CDCC","parts":{"hash":"07F449C5460D97F2B599A242F59235293A74A569A34C0369E11C360699A80DCA","total":1}} height=115245 module=consensus peer=8855d5696c4aec427051bd2ed3262e7e3a37f34d round=0 server=node type=2
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Replay: Vote blockID={"hash":"06C846E8FD8D3736293BECDD17B51F6DED41B5E02792FDC193EFB251AB47CDCC","parts":{"hash":"07F449C5460D97F2B599A242F59235293A74A569A34C0369E11C360699A80DCA","total":1}} height=115245 module=consensus peer=8855d5696c4aec427051bd2ed3262e7e3a37f34d round=0 server=node type=2
May 19 16:22:56 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:22PM INF Replay: Vote blockID={"hash":"06C846E8FD8D3736293BECDD17B51F6DED41B5E02792FDC193EFB251AB47CDCC","parts":{"hash":"07F449C5460D97F2B599A242F59235293A74A569A34C0369E11C360699A80DCA","total":1}} height=115245 module=consensus peer=8855d5696c4aec427051bd2ed3262e7e3a37f34d round=0 server=node type=2
~~~

## Restart 2
~~~bash

~~~
