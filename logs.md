# Restart your validator three times during Mission 2

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

## Restart 2 2023-05-16 00:28:03 CEST
~~~bash
sudo systemctl restart humansd && sudo journalctl -u humansd -f
-- Logs begin at Tue 2023-05-16 00:28:03 CEST. --
May 19 16:32:46 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:32PM INF service stop impl={"Logger":{},"Switch":{"Logger":{}}} module=blockchain msg={} server=node
May 19 16:32:46 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:32PM INF Saving AddrBook to file book=/root/.humansd/config/addrbook.json module=p2p server=node size=121
May 19 16:32:46 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:32PM ERR Error stopping pool err="already stopped" module=blockchain server=node
May 19 16:32:46 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:32PM ERR Stopped accept routine, as transport is closed module=p2p numPeers=0 server=node
May 19 16:32:46 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:32PM INF Closing rpc listener listener={"Listener":{}} server=node
May 19 16:32:46 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:32PM INF RPC HTTP server stopped err="accept tcp [::]:26657: use of closed network connection" module=rpc-server server=node
May 19 16:32:46 Ubuntu-2004-focal-64-minimal humansd[3503604]: 4:32PM ERR Error serving server err="accept tcp [::]:26657: use of closed network connection" server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal systemd[1]: humansd.service: Succeeded.
May 19 16:32:47 Ubuntu-2004-focal-64-minimal systemd[1]: Stopped Humans node.
May 19 16:32:47 Ubuntu-2004-focal-64-minimal systemd[1]: Started Humans node.
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Unlocking keyring
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF starting ABCI with Tendermint
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF starting node with ABCI Tendermint in-process
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=multiAppConn module=proxy msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start connection=query impl=localClient module=abci-client msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start connection=snapshot impl=localClient module=abci-client msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start connection=mempool impl=localClient module=abci-client msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start connection=consensus impl=localClient module=abci-client msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=EventBus module=events msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=PubSub module=pubsub msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=IndexerService module=txindex msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF ABCI Handshake App Info hash="O��f�\x04� m0ex\"�\x10��\x1a��J�V�\f�;�ɩ��" height=115330 module=consensus protocol-version=0 server=node software-version=0.2.2
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF ABCI Replay Blocks appHeight=115330 module=consensus server=node stateHeight=115330 storeHeight=115330
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Completed ABCI Handshake - CometBFT and App are synced appHash="O��f�\x04� m0ex\"�\x10��\x1a��J�V�\f�;�ɩ��" appHeight=115330 module=consensus server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Version info abci=0.17.0 block=11 cmtbft_version=0.34.27 commit_hash= p2p=8 server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF This node is a validator addr=A5AD742A8FB77530A69CC9B772D7D2610CA29907 module=consensus pubKey=uhkgaTMe+rHTTB8fV76uLJCI4AEPj55WjnmJgy17mDU= server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF P2P Node ID ID=df5cb643d8aeade8ef288a3dd90e4fd8220954ba file=/root/.humansd/config/node_key.json module=p2p server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Adding persistent peers addrs=[] module=p2p server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Adding unconditional peer ids ids=[] module=p2p server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Add our address to book addr={"id":"df5cb643d8aeade8ef288a3dd90e4fd8220954ba","ip":"0.0.0.0","port":36656} book=/root/.humansd/config/addrbook.json module=p2p server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Add our address to book addr={"id":"df5cb643d8aeade8ef288a3dd90e4fd8220954ba","ip":"0.0.0.0","port":36656} book=/root/.humansd/config/addrbook.json module=p2p server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=Node msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Starting pprof server laddr=localhost:6061 server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="P2P Switch" module=p2p msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF serve module=rpc-server msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=BlockchainReactor module=blockchain msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=BlockPool module=blockchain msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=ConsensusReactor module=consensus msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Reactor  module=consensus server=node waitSync=true
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=Evidence module=evidence msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=StateSync module=statesync msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=PEX module=pex msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start book=/root/.humansd/config/addrbook.json impl=AddrBook module=p2p msg={} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Saving AddrBook to file book=/root/.humansd/config/addrbook.json module=p2p server=node size=121
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Ensure peers module=pex numDialing=0 numInPeers=0 numOutPeers=0 numToDial=10 server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{144.76.45.59:26656} de3cd5f6c726935c4c0fdb1e6bd5b705074c637c out}" module=p2p msg={} peer={"id":"de3cd5f6c726935c4c0fdb1e6bd5b705074c637c","ip":"144.76.45.59","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{144.76.45.59:26656} module=p2p msg={} peer={"id":"de3cd5f6c726935c4c0fdb1e6bd5b705074c637c","ip":"144.76.45.59","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{78.46.80.79:26656} 497886715ac23475f7428bd177b9fa53ff886a8d out}" module=p2p msg={} peer={"id":"497886715ac23475f7428bd177b9fa53ff886a8d","ip":"78.46.80.79","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{78.46.80.79:26656} module=p2p msg={} peer={"id":"497886715ac23475f7428bd177b9fa53ff886a8d","ip":"78.46.80.79","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{178.23.126.70:26656} fa9eb901a01430d928e71162151992c7afb51d62 out}" module=p2p msg={} peer={"id":"fa9eb901a01430d928e71162151992c7afb51d62","ip":"178.23.126.70","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{178.23.126.70:26656} module=p2p msg={} peer={"id":"fa9eb901a01430d928e71162151992c7afb51d62","ip":"178.23.126.70","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{65.108.231.124:17656} 6ce9a9acc23594ec75516617647286fe546f83ca out}" module=p2p msg={} peer={"id":"6ce9a9acc23594ec75516617647286fe546f83ca","ip":"65.108.231.124","port":17656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{65.108.231.124:17656} module=p2p msg={} peer={"id":"6ce9a9acc23594ec75516617647286fe546f83ca","ip":"65.108.231.124","port":17656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{65.109.84.33:26656} 5b92ede5e88c5029d6c7b3b360b9cf59051ce409 out}" module=p2p msg={} peer={"id":"5b92ede5e88c5029d6c7b3b360b9cf59051ce409","ip":"65.109.84.33","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{65.109.84.33:26656} module=p2p msg={} peer={"id":"5b92ede5e88c5029d6c7b3b360b9cf59051ce409","ip":"65.109.84.33","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{212.47.234.144:26656} 19230fad7145e6fe80566a72f66b9ca3ec3f04d5 out}" module=p2p msg={} peer={"id":"19230fad7145e6fe80566a72f66b9ca3ec3f04d5","ip":"212.47.234.144","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{212.47.234.144:26656} module=p2p msg={} peer={"id":"19230fad7145e6fe80566a72f66b9ca3ec3f04d5","ip":"212.47.234.144","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF starting API server... server=api
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF serve msg={} server=api
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{91.194.30.203:26656} b1639fb460c9f55bb3acc3006df64ac5013f1412 out}" module=p2p msg={} peer={"id":"b1639fb460c9f55bb3acc3006df64ac5013f1412","ip":"91.194.30.203","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{91.194.30.203:26656} module=p2p msg={} peer={"id":"b1639fb460c9f55bb3acc3006df64ac5013f1412","ip":"91.194.30.203","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Connection is closed @ recvRoutine (likely by the other side) conn={"Logger":{}} module=p2p peer={"id":"6ce9a9acc23594ec75516617647286fe546f83ca","ip":"65.108.231.124","port":17656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service stop impl={"Logger":{}} module=p2p msg={} peer={"id":"6ce9a9acc23594ec75516617647286fe546f83ca","ip":"65.108.231.124","port":17656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM ERR Stopping peer for error err=EOF module=p2p peer={"Data":{},"Logger":{}} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service stop impl={"Data":{},"Logger":{}} module=p2p msg={} peer={"id":"6ce9a9acc23594ec75516617647286fe546f83ca","ip":"65.108.231.124","port":17656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{159.69.69.183:26656} ee8a0664518c5ef5078ad2251275d5689fcf96fb out}" module=p2p msg={} peer={"id":"ee8a0664518c5ef5078ad2251275d5689fcf96fb","ip":"159.69.69.183","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{159.69.69.183:26656} module=p2p msg={} peer={"id":"ee8a0664518c5ef5078ad2251275d5689fcf96fb","ip":"159.69.69.183","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{144.76.97.35:26656} 733ffab95701aeebbc3021e827a7ef5f5c0dd93c out}" module=p2p msg={} peer={"id":"733ffab95701aeebbc3021e827a7ef5f5c0dd93c","ip":"144.76.97.35","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{144.76.97.35:26656} module=p2p msg={} peer={"id":"733ffab95701aeebbc3021e827a7ef5f5c0dd93c","ip":"144.76.97.35","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{128.140.56.206:26656} e6489cf86b51fa37cae968ccbbda1da03b742a5e out}" module=p2p msg={} peer={"id":"e6489cf86b51fa37cae968ccbbda1da03b742a5e","ip":"128.140.56.206","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{128.140.56.206:26656} module=p2p msg={} peer={"id":"e6489cf86b51fa37cae968ccbbda1da03b742a5e","ip":"128.140.56.206","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{162.55.173.57:26656} f05366147458d2d09ff525f8b4258a7978f72991 out}" module=p2p msg={} peer={"id":"f05366147458d2d09ff525f8b4258a7978f72991","ip":"162.55.173.57","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{162.55.173.57:26656} module=p2p msg={} peer={"id":"f05366147458d2d09ff525f8b4258a7978f72991","ip":"162.55.173.57","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{138.201.121.185:26656} 6271d80b8fc42da3a2825cc5ef75818dd52423d1 out}" module=p2p msg={} peer={"id":"6271d80b8fc42da3a2825cc5ef75818dd52423d1","ip":"138.201.121.185","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{138.201.121.185:26656} module=p2p msg={} peer={"id":"6271d80b8fc42da3a2825cc5ef75818dd52423d1","ip":"138.201.121.185","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{94.237.27.19:26656} 42f95015c31c7814b6a0a717fd8c63d15f896e88 out}" module=p2p msg={} peer={"id":"42f95015c31c7814b6a0a717fd8c63d15f896e88","ip":"94.237.27.19","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{94.237.27.19:26656} module=p2p msg={} peer={"id":"42f95015c31c7814b6a0a717fd8c63d15f896e88","ip":"94.237.27.19","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{135.181.142.117:26656} 459bcaea161d20cddcdead811d282bd495446cbb out}" module=p2p msg={} peer={"id":"459bcaea161d20cddcdead811d282bd495446cbb","ip":"135.181.142.117","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{135.181.142.117:26656} module=p2p msg={} peer={"id":"459bcaea161d20cddcdead811d282bd495446cbb","ip":"135.181.142.117","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{65.109.116.95:26656} 35ad999115e2a58540f6cf3bc3b90cc3adc9debc out}" module=p2p msg={} peer={"id":"35ad999115e2a58540f6cf3bc3b90cc3adc9debc","ip":"65.109.116.95","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{65.109.116.95:26656} module=p2p msg={} peer={"id":"35ad999115e2a58540f6cf3bc3b90cc3adc9debc","ip":"65.109.116.95","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{65.109.155.238:29656} 6e2dac7a826fa2c21867dc6620b5945574a89865 out}" module=p2p msg={} peer={"id":"6e2dac7a826fa2c21867dc6620b5945574a89865","ip":"65.109.155.238","port":29656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{65.109.155.238:29656} module=p2p msg={} peer={"id":"6e2dac7a826fa2c21867dc6620b5945574a89865","ip":"65.109.155.238","port":29656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{65.21.200.54:26656} 907cb9da5d7d7182a80a6e38aad59bd067059bb3 out}" module=p2p msg={} peer={"id":"907cb9da5d7d7182a80a6e38aad59bd067059bb3","ip":"65.21.200.54","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{65.21.200.54:26656} module=p2p msg={} peer={"id":"907cb9da5d7d7182a80a6e38aad59bd067059bb3","ip":"65.21.200.54","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{38.146.3.209:26656} 6c2581bce457207a8d29895216a06f0f98d39599 out}" module=p2p msg={} peer={"id":"6c2581bce457207a8d29895216a06f0f98d39599","ip":"38.146.3.209","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{38.146.3.209:26656} module=p2p msg={} peer={"id":"6c2581bce457207a8d29895216a06f0f98d39599","ip":"38.146.3.209","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{143.110.190.223:26656} 5ca0389db000da1ce87d992816a4aefa387c3998 out}" module=p2p msg={} peer={"id":"5ca0389db000da1ce87d992816a4aefa387c3998","ip":"143.110.190.223","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{143.110.190.223:26656} module=p2p msg={} peer={"id":"5ca0389db000da1ce87d992816a4aefa387c3998","ip":"143.110.190.223","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{51.79.101.159:26656} be5158df5152ec7e6a4eca04c89e40494d19927c out}" module=p2p msg={} peer={"id":"be5158df5152ec7e6a4eca04c89e40494d19927c","ip":"51.79.101.159","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{51.79.101.159:26656} module=p2p msg={} peer={"id":"be5158df5152ec7e6a4eca04c89e40494d19927c","ip":"51.79.101.159","port":26656} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl="Peer{MConn{38.146.3.210:18456} ef4cf8c00b34de7a8c1eba725ac91a93c085781c out}" module=p2p msg={} peer={"id":"ef4cf8c00b34de7a8c1eba725ac91a93c085781c","ip":"38.146.3.210","port":18456} server=node
May 19 16:32:47 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=MConn{38.146.3.210:18456} module=p2p msg={} peer={"id":"ef4cf8c00b34de7a8c1eba725ac91a93c085781c","ip":"38.146.3.210","port":18456} server=node
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Time to switch to consensus reactor! height=115331 module=blockchain server=node
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service stop impl={"Logger":{}} module=blockchain msg={} server=node
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF SwitchToConsensus module=consensus server=node
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=ConsensusState module=consensus msg={} server=node
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=baseWAL module=consensus msg={} server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=Group module=consensus msg={} server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF service start impl=TimeoutTicker module=consensus msg={} server=node
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Searching for height height=115331 max=5691 min=5594 module=consensus server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Searching for height height=115330 max=5691 min=5594 module=consensus server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Found height=115330 index=5691 module=consensus server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Catchup by replaying consensus messages height=115331 module=consensus server=node
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Replay: New Step height=115331 module=consensus round=0 server=node step=RoundStepNewHeight
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Replay: Vote blockID={"hash":"4A1761A315623DD2A094A2D8D9C93645415E3E0A47FD880BB268B41D618F4500","parts":{"hash":"F0655C89589A7BFF45B7566F38D3CB21575CE8B03471E7B2E87F8CE6FDF6540F","total":1}} height=115330 module=consensus peer=459bcaea161d20cddcdead811d282bd495446cbb round=0 server=node type=2
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Replay: Vote blockID={"hash":"4A1761A315623DD2A094A2D8D9C93645415E3E0A47FD880BB268B41D618F4500","parts":{"hash":"F0655C89589A7BFF45B7566F38D3CB21575CE8B03471E7B2E87F8CE6FDF6540F","total":1}} height=115330 module=consensus peer=459bcaea161d20cddcdead811d282bd495446cbb round=0 server=node type=2
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Replay: Vote blockID={"hash":"4A1761A315623DD2A094A2D8D9C93645415E3E0A47FD880BB268B41D618F4500","parts":{"hash":"F0655C89589A7BFF45B7566F38D3CB21575CE8B03471E7B2E87F8CE6FDF6540F","total":1}} height=115330 module=consensus peer=459bcaea161d20cddcdead811d282bd495446cbb round=0 server=node type=2
May 19 16:32:48 Ubuntu-2004-focal-64-minimal humansd[3510438]: 4:32PM INF Replay: Vote blockID={"hash":"4A1761A315623DD2A094A2D8D9C93645415E3E0A47FD880BB268B41D618F4500","parts":{"hash":"F0655C89589A7BFF45B7566F38D3CB21575CE8B03471E7B2E87F8CE6FDF6540F","total":1}} height=115330 module=consensus peer=6c2581bce457207a8d29895216a06f0f98d39599 round=0 server=node type=2
~~~

## Restart 3 2023-05-16 00:28:03 CEST
~~~bash
sudo systemctl restart humansd && sudo journalctl -u humansd -f
-- Logs begin at Tue 2023-05-16 00:28:03 CEST. --
May 19 16:35:22 Ubuntu-2004-focal-64-minimal humansd[3512259]: 4:35PM INF Replay: Vote blockID={"hash":"","parts":{"hash":"","total":0}} height=115355 module=consensus peer=6c2581bce457207a8d29895216a06f0f98d39599 round=0 server=node type=1
May 19 16:35:22 Ubuntu-2004-focal-64-minimal humansd[3512259]: 4:35PM INF Replay: Vote blockID={"hash":"","parts":{"hash":"","total":0}} height=115355 module=consensus peer=6c2581bce457207a8d29895216a06f0f98d39599 round=0 server=node type=1
May 19 16:35:22 Ubuntu-2004-focal-64-minimal humansd[3512259]: 4:35PM INF Replay: Vote blockID={"hash":"","parts":{"hash":"","total":0}} height=115355 module=consensus peer=be5158df5152ec7e6a4eca04c89e40494d19927c round=0 server=node type=1
May 19 16:35:22 Ubuntu-2004-focal-64-minimal humansd[3512259]: 4:35PM INF Replay: Vote blockID={"hash":"","parts":{"hash":"","total":0}} height=115355 module=consensus peer=be5158df5152ec7e6a4eca04c89e40494d19927c round=0 server=node type=1
May 19 16:35:22 Ubuntu-2004-focal-64-minimal humansd[3512259]: 4:35PM INF Replay: Vote blockID={"hash":"","parts":{"hash":"","total":0}} height=115355 module=consensus peer=ef4cf8c00b34de7a8c1eba725ac91a93c085781c round=0 server=node type=1
May 19 16:35:22 Ubuntu-2004-focal-64-minimal humansd[3512259]: 4:35PM INF Replay: Done module=consensus server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal systemd[1]: Stopping Humans node...
May 19 16:35:27 Ubuntu-2004-focal-64-minimal systemd[1]: humansd.service: Succeeded.
May 19 16:35:27 Ubuntu-2004-focal-64-minimal systemd[1]: Stopped Humans node.
May 19 16:35:27 Ubuntu-2004-focal-64-minimal systemd[1]: Started Humans node.
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Unlocking keyring
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF starting ABCI with Tendermint
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF starting node with ABCI Tendermint in-process
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=multiAppConn module=proxy msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start connection=query impl=localClient module=abci-client msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start connection=snapshot impl=localClient module=abci-client msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start connection=mempool impl=localClient module=abci-client msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start connection=consensus impl=localClient module=abci-client msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=EventBus module=events msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=PubSub module=pubsub msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=IndexerService module=txindex msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF ABCI Handshake App Info hash="\x05s��\x05\x13��\x1a�m\vC����{}{!��{\x05~�\f���\x04" height=115354 module=consensus protocol-version=0 server=node software-version=0.2.2
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF ABCI Replay Blocks appHeight=115354 module=consensus server=node stateHeight=115354 storeHeight=115354
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Completed ABCI Handshake - CometBFT and App are synced appHash="\x05s��\x05\x13��\x1a�m\vC����{}{!��{\x05~�\f���\x04" appHeight=115354 module=consensus server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Version info abci=0.17.0 block=11 cmtbft_version=0.34.27 commit_hash= p2p=8 server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF This node is a validator addr=A5AD742A8FB77530A69CC9B772D7D2610CA29907 module=consensus pubKey=uhkgaTMe+rHTTB8fV76uLJCI4AEPj55WjnmJgy17mDU= server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF P2P Node ID ID=df5cb643d8aeade8ef288a3dd90e4fd8220954ba file=/root/.humansd/config/node_key.json module=p2p server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Adding persistent peers addrs=[] module=p2p server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Adding unconditional peer ids ids=[] module=p2p server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Add our address to book addr={"id":"df5cb643d8aeade8ef288a3dd90e4fd8220954ba","ip":"0.0.0.0","port":36656} book=/root/.humansd/config/addrbook.json module=p2p server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Add our address to book addr={"id":"df5cb643d8aeade8ef288a3dd90e4fd8220954ba","ip":"0.0.0.0","port":36656} book=/root/.humansd/config/addrbook.json module=p2p server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=Node msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Starting pprof server laddr=localhost:6061 server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="P2P Switch" module=p2p msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=ConsensusReactor module=consensus msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Reactor  module=consensus server=node waitSync=true
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=Evidence module=evidence msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=StateSync module=statesync msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF serve module=rpc-server msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=PEX module=pex msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start book=/root/.humansd/config/addrbook.json impl=AddrBook module=p2p msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=BlockchainReactor module=blockchain msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=BlockPool module=blockchain msg={} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Ensure peers module=pex numDialing=0 numInPeers=0 numOutPeers=0 numToDial=10 server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Saving AddrBook to file book=/root/.humansd/config/addrbook.json module=p2p server=node size=121
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{78.46.80.79:26656} 497886715ac23475f7428bd177b9fa53ff886a8d out}" module=p2p msg={} peer={"id":"497886715ac23475f7428bd177b9fa53ff886a8d","ip":"78.46.80.79","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{78.46.64.59:26656} a41f29c2d498b232c18f75364e38cee06fac198d out}" module=p2p msg={} peer={"id":"a41f29c2d498b232c18f75364e38cee06fac198d","ip":"78.46.64.59","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{78.46.80.79:26656} module=p2p msg={} peer={"id":"497886715ac23475f7428bd177b9fa53ff886a8d","ip":"78.46.80.79","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{78.46.64.59:26656} module=p2p msg={} peer={"id":"a41f29c2d498b232c18f75364e38cee06fac198d","ip":"78.46.64.59","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{94.237.27.19:26656} 42f95015c31c7814b6a0a717fd8c63d15f896e88 out}" module=p2p msg={} peer={"id":"42f95015c31c7814b6a0a717fd8c63d15f896e88","ip":"94.237.27.19","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{94.237.27.19:26656} module=p2p msg={} peer={"id":"42f95015c31c7814b6a0a717fd8c63d15f896e88","ip":"94.237.27.19","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{162.19.31.150:26656} 0ae23e03040dd3e3a6c3a2326c62a206f531d671 out}" module=p2p msg={} peer={"id":"0ae23e03040dd3e3a6c3a2326c62a206f531d671","ip":"162.19.31.150","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{162.19.31.150:26656} module=p2p msg={} peer={"id":"0ae23e03040dd3e3a6c3a2326c62a206f531d671","ip":"162.19.31.150","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{178.23.126.70:26656} fa9eb901a01430d928e71162151992c7afb51d62 out}" module=p2p msg={} peer={"id":"fa9eb901a01430d928e71162151992c7afb51d62","ip":"178.23.126.70","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{178.23.126.70:26656} module=p2p msg={} peer={"id":"fa9eb901a01430d928e71162151992c7afb51d62","ip":"178.23.126.70","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{65.108.231.124:17656} 6ce9a9acc23594ec75516617647286fe546f83ca out}" module=p2p msg={} peer={"id":"6ce9a9acc23594ec75516617647286fe546f83ca","ip":"65.108.231.124","port":17656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{135.181.18.112:55686} 2685f8e77fec93c99a55f2adb13835a50124d04e out}" module=p2p msg={} peer={"id":"2685f8e77fec93c99a55f2adb13835a50124d04e","ip":"135.181.18.112","port":55686} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{65.108.231.124:17656} module=p2p msg={} peer={"id":"6ce9a9acc23594ec75516617647286fe546f83ca","ip":"65.108.231.124","port":17656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{135.181.18.112:55686} module=p2p msg={} peer={"id":"2685f8e77fec93c99a55f2adb13835a50124d04e","ip":"135.181.18.112","port":55686} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{95.217.200.36:26656} 2f6cc8b0b255745d71c358351ddde1faa350b0be out}" module=p2p msg={} peer={"id":"2f6cc8b0b255745d71c358351ddde1faa350b0be","ip":"95.217.200.36","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{95.217.200.36:26656} module=p2p msg={} peer={"id":"2f6cc8b0b255745d71c358351ddde1faa350b0be","ip":"95.217.200.36","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF starting API server... server=api
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF serve msg={} server=api
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Connection is closed @ recvRoutine (likely by the other side) conn={"Logger":{}} module=p2p peer={"id":"6ce9a9acc23594ec75516617647286fe546f83ca","ip":"65.108.231.124","port":17656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service stop impl={"Logger":{}} module=p2p msg={} peer={"id":"6ce9a9acc23594ec75516617647286fe546f83ca","ip":"65.108.231.124","port":17656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM ERR Stopping peer for error err=EOF module=p2p peer={"Data":{},"Logger":{}} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service stop impl={"Data":{},"Logger":{}} module=p2p msg={} peer={"id":"6ce9a9acc23594ec75516617647286fe546f83ca","ip":"65.108.231.124","port":17656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{144.76.45.59:26656} de3cd5f6c726935c4c0fdb1e6bd5b705074c637c out}" module=p2p msg={} peer={"id":"de3cd5f6c726935c4c0fdb1e6bd5b705074c637c","ip":"144.76.45.59","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{144.76.45.59:26656} module=p2p msg={} peer={"id":"de3cd5f6c726935c4c0fdb1e6bd5b705074c637c","ip":"144.76.45.59","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{138.201.121.185:26656} 6271d80b8fc42da3a2825cc5ef75818dd52423d1 out}" module=p2p msg={} peer={"id":"6271d80b8fc42da3a2825cc5ef75818dd52423d1","ip":"138.201.121.185","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{138.201.121.185:26656} module=p2p msg={} peer={"id":"6271d80b8fc42da3a2825cc5ef75818dd52423d1","ip":"138.201.121.185","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{128.140.56.206:26656} e6489cf86b51fa37cae968ccbbda1da03b742a5e out}" module=p2p msg={} peer={"id":"e6489cf86b51fa37cae968ccbbda1da03b742a5e","ip":"128.140.56.206","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{128.140.56.206:26656} module=p2p msg={} peer={"id":"e6489cf86b51fa37cae968ccbbda1da03b742a5e","ip":"128.140.56.206","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{51.79.101.159:26656} be5158df5152ec7e6a4eca04c89e40494d19927c out}" module=p2p msg={} peer={"id":"be5158df5152ec7e6a4eca04c89e40494d19927c","ip":"51.79.101.159","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{51.79.101.159:26656} module=p2p msg={} peer={"id":"be5158df5152ec7e6a4eca04c89e40494d19927c","ip":"51.79.101.159","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{65.21.200.54:26656} 907cb9da5d7d7182a80a6e38aad59bd067059bb3 out}" module=p2p msg={} peer={"id":"907cb9da5d7d7182a80a6e38aad59bd067059bb3","ip":"65.21.200.54","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{65.21.200.54:26656} module=p2p msg={} peer={"id":"907cb9da5d7d7182a80a6e38aad59bd067059bb3","ip":"65.21.200.54","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{135.181.113.225:26656} ceba57f1376d4949cc0419918d110f0085b24b25 out}" module=p2p msg={} peer={"id":"ceba57f1376d4949cc0419918d110f0085b24b25","ip":"135.181.113.225","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{135.181.113.225:26656} module=p2p msg={} peer={"id":"ceba57f1376d4949cc0419918d110f0085b24b25","ip":"135.181.113.225","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{65.109.116.95:26656} 35ad999115e2a58540f6cf3bc3b90cc3adc9debc out}" module=p2p msg={} peer={"id":"35ad999115e2a58540f6cf3bc3b90cc3adc9debc","ip":"65.109.116.95","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{65.109.116.95:26656} module=p2p msg={} peer={"id":"35ad999115e2a58540f6cf3bc3b90cc3adc9debc","ip":"65.109.116.95","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{69.197.6.24:26656} 22ccc03acda4e7230f779dc3955a0097a32c358e out}" module=p2p msg={} peer={"id":"22ccc03acda4e7230f779dc3955a0097a32c358e","ip":"69.197.6.24","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{69.197.6.24:26656} module=p2p msg={} peer={"id":"22ccc03acda4e7230f779dc3955a0097a32c358e","ip":"69.197.6.24","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{143.110.190.223:26656} 5ca0389db000da1ce87d992816a4aefa387c3998 out}" module=p2p msg={} peer={"id":"5ca0389db000da1ce87d992816a4aefa387c3998","ip":"143.110.190.223","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{143.110.190.223:26656} module=p2p msg={} peer={"id":"5ca0389db000da1ce87d992816a4aefa387c3998","ip":"143.110.190.223","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{206.125.33.0:26656} d7eb0e65cecbeeaa649b0a2fdf95ca2fb9f0cc3e out}" module=p2p msg={} peer={"id":"d7eb0e65cecbeeaa649b0a2fdf95ca2fb9f0cc3e","ip":"206.125.33.0","port":26656} server=node
May 19 16:35:27 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{206.125.33.0:26656} module=p2p msg={} peer={"id":"d7eb0e65cecbeeaa649b0a2fdf95ca2fb9f0cc3e","ip":"206.125.33.0","port":26656} server=node
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl="Peer{MConn{103.180.28.79:26656} 36f956fa2fe317a5d3163d0b6c7b104e33aa62e9 out}" module=p2p msg={} peer={"id":"36f956fa2fe317a5d3163d0b6c7b104e33aa62e9","ip":"103.180.28.79","port":26656} server=node
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=MConn{103.180.28.79:26656} module=p2p msg={} peer={"id":"36f956fa2fe317a5d3163d0b6c7b104e33aa62e9","ip":"103.180.28.79","port":26656} server=node
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Time to switch to consensus reactor! height=115355 module=blockchain server=node
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service stop impl={"Logger":{}} module=blockchain msg={} server=node
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF SwitchToConsensus module=consensus server=node
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=ConsensusState module=consensus msg={} server=node
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=baseWAL module=consensus msg={} server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=Group module=consensus msg={} server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF service start impl=TimeoutTicker module=consensus msg={} server=node
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Searching for height height=115355 max=5693 min=5596 module=consensus server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Searching for height height=115354 max=5693 min=5596 module=consensus server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Found height=115354 index=5693 module=consensus server=node wal=/root/.humansd/data/cs.wal/wal
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Catchup by replaying consensus messages height=115355 module=consensus server=node
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Replay: New Step height=115355 module=consensus round=0 server=node step=RoundStepNewHeight
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Replay: Vote blockID={"hash":"67B9723C34A7AA475B08055E8176A53B4AD641EE01CA362DD1EFE293368A1803","parts":{"hash":"0809D0A39C9F4B135C71D135CFC713291A2E75C3EA7802186AD67634C87AF5D8","total":1}} height=115354 module=consensus peer=f05366147458d2d09ff525f8b4258a7978f72991 round=0 server=node type=2
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Replay: Vote blockID={"hash":"67B9723C34A7AA475B08055E8176A53B4AD641EE01CA362DD1EFE293368A1803","parts":{"hash":"0809D0A39C9F4B135C71D135CFC713291A2E75C3EA7802186AD67634C87AF5D8","total":1}} height=115354 module=consensus peer=f05366147458d2d09ff525f8b4258a7978f72991 round=0 server=node type=2
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Replay: Vote blockID={"hash":"67B9723C34A7AA475B08055E8176A53B4AD641EE01CA362DD1EFE293368A1803","parts":{"hash":"0809D0A39C9F4B135C71D135CFC713291A2E75C3EA7802186AD67634C87AF5D8","total":1}} height=115354 module=consensus peer=f05366147458d2d09ff525f8b4258a7978f72991 round=0 server=node type=2
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Replay: Vote blockID={"hash":"67B9723C34A7AA475B08055E8176A53B4AD641EE01CA362DD1EFE293368A1803","parts":{"hash":"0809D0A39C9F4B135C71D135CFC713291A2E75C3EA7802186AD67634C87AF5D8","total":1}} height=115354 module=consensus peer=f05366147458d2d09ff525f8b4258a7978f72991 round=0 server=node type=2
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Replay: Vote blockID={"hash":"67B9723C34A7AA475B08055E8176A53B4AD641EE01CA362DD1EFE293368A1803","parts":{"hash":"0809D0A39C9F4B135C71D135CFC713291A2E75C3EA7802186AD67634C87AF5D8","total":1}} height=115354 module=consensus peer=f05366147458d2d09ff525f8b4258a7978f72991 round=0 server=node type=1
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Replay: Vote blockID={"hash":"67B9723C34A7AA475B08055E8176A53B4AD641EE01CA362DD1EFE293368A1803","parts":{"hash":"0809D0A39C9F4B135C71D135CFC713291A2E75C3EA7802186AD67634C87AF5D8","total":1}} height=115354 module=consensus peer=f05366147458d2d09ff525f8b4258a7978f72991 round=0 server=node type=1
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Replay: Vote blockID={"hash":"67B9723C34A7AA475B08055E8176A53B4AD641EE01CA362DD1EFE293368A1803","parts":{"hash":"0809D0A39C9F4B135C71D135CFC713291A2E75C3EA7802186AD67634C87AF5D8","total":1}} height=115354 module=consensus peer=fa9eb901a01430d928e71162151992c7afb51d62 round=0 server=node type=2
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Replay: Vote blockID={"hash":"67B9723C34A7AA475B08055E8176A53B4AD641EE01CA362DD1EFE293368A1803","parts":{"hash":"0809D0A39C9F4B135C71D135CFC713291A2E75C3EA7802186AD67634C87AF5D8","total":1}} height=115354 module=consensus peer=fa9eb901a01430d928e71162151992c7afb51d62 round=0 server=node type=2
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Replay: Vote blockID={"hash":"67B9723C34A7AA475B08055E8176A53B4AD641EE01CA362DD1EFE293368A1803","parts":{"hash":"0809D0A39C9F4B135C71D135CFC713291A2E75C3EA7802186AD67634C87AF5D8","total":1}} height=115354 module=consensus peer=fa9eb901a01430d928e71162151992c7afb51d62 round=0 server=node type=2
May 19 16:35:28 Ubuntu-2004-focal-64-minimal humansd[3512367]: 4:35PM INF Replay: Vote blockID={"hash":"67B9723C34A7AA475B08055E8176A53B4AD641EE01CA362DD1EFE293368A1803","parts":{"hash":"0809D0A39C9F4B135C71D135CFC713291A2E75C3EA7802186AD67634C87AF5D8","total":1}} height=115354 module=consensus peer=fa9eb901a01430d928e71162151992c7afb51d62 round=0 server=node type=2
~~~
