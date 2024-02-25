**`IBC Namada (shielded-expedition.88f17d1d14) <> Cosmos (theta-testnet-001)`**

```
Namada (shielded-expedition.88f17d1d14):
   channel_id:    channel-440
   client_id:     07-tendermint-1557
   connection_id: connection-670
   port_id:       transfer
Creation address: tnam1qpxugj9cmdu05269trs954p9kxh9td0mpcylnkk2
```
```
Cosmos (theta-testnet-001): 
   channel_id:    channel-3878
   client_id:     07-tendermint-3202
   connection_id: connection-3381
   port_id:       transfer
Creation address: cosmos1knygypaqjav7q8wpu6lpqjfhdg3a5axzccmqm6
```

**`Test transactions:`**

**Namada (shielded-expedition.88f17d1d14) > Cosmos (theta-testnet-001)**
https://extended-nebb.kintsugi.tech/player/tpknam1qzk6u8wh6qhqc7j9etxdlz9wqczyh2vsm44hgs6dphed3vp0uk2tvl8lcm5

![image](https://github.com/DmitriiRabeckii/ibc/assets/25347359/1bd5c352-7615-49e9-9b56-88e85c050b00)

**Cosmos (theta-testnet-001) > Namada (shielded-expedition.88f17d1d14)**
https://www.mintscan.io/cosmoshub-testnet/tx/0A3FDE816A0A22DE44939E971B0EABDACF8C726818AA24F4AEF7EB72BF2E5FA9?height=20461901

**`LOGS:`**
```
2024-02-25T18:37:30.931781Z  INFO ThreadId(01) running Hermes v1.7.4+38f41c6
2024-02-25T18:37:31.413456Z  INFO ThreadId(01) Creating new clients, new connection, and a new channel with order ORDER_UNORDERED
2024-02-25T18:37:49.861202Z  INFO ThreadId(01) foreign_client.create{client=theta-testnet-001->shielded-expedition.88f17d1d14:07-tendermint-0}: 🍭 client was created successfully id=07-tendermint-1557
2024-02-25T18:37:53.554587Z  INFO ThreadId(01) foreign_client.create{client=shielded-expedition.88f17d1d14->theta-testnet-001:07-tendermint-0}: 🍭 client was created successfully id=07-tendermint-3202
2024-02-25T18:38:14.546488Z  INFO ThreadId(01) 🥂 shielded-expedition.88f17d1d14 => OpenInitConnection(OpenInit { Attributes { connection_id: connection-670, client_id: 07-tendermint-1557, counterparty_connection_id: None, counterparty_client_id: 07-tendermint-3202 } }) at height 0-65887
2024-02-25T18:39:04.953988Z  INFO ThreadId(01) 🥂 theta-testnet-001 => OpenTryConnection(OpenTry { Attributes { connection_id: connection-3381, client_id: 07-tendermint-3202, counterparty_connection_id: connection-670, counterparty_client_id: 07-tendermint-1557 } }) at height 0-20459080
2024-02-25T18:39:54.081458Z  INFO ThreadId(01) 🥂 shielded-expedition.88f17d1d14 => OpenAckConnection(OpenAck { Attributes { connection_id: connection-670, client_id: 07-tendermint-1557, counterparty_connection_id: connection-3381, counterparty_client_id: 07-tendermint-3202 } }) at height 0-65896
2024-02-25T18:40:11.569636Z  INFO ThreadId(01) 🥂 theta-testnet-001 => OpenConfirmConnection(OpenConfirm { Attributes { connection_id: connection-3381, client_id: 07-tendermint-3202, counterparty_connection_id: connection-670, counterparty_client_id: 07-tendermint-1557 } }) at height 0-20459092
2024-02-25T18:40:17.896144Z  INFO ThreadId(01) connection handshake already finished for Connection { delay_period: 0ns, a_side: ConnectionSide { chain: BaseChainHandle { chain_id: shielded-expedition.88f17d1d14 }, client_id: 07-tendermint-1557, connection_id: connection-670 }, b_side: ConnectionSide { chain: BaseChainHandle { chain_id: theta-testnet-001 }, client_id: 07-tendermint-3202, connection_id: connection-3381 } }
2024-02-25T18:40:37.227483Z  INFO ThreadId(01) 🎊  shielded-expedition.88f17d1d14 => OpenInitChannel(OpenInit { port_id: transfer, channel_id: channel-440, connection_id: None, counterparty_port_id: transfer, counterparty_channel_id: None }) at height 0-65900
2024-02-25T18:40:55.796585Z  INFO ThreadId(01) 🎊  theta-testnet-001 => OpenTryChannel(OpenTry { port_id: transfer, channel_id: channel-3878, connection_id: connection-3381, counterparty_port_id: transfer, counterparty_channel_id: channel-440 }) at height 0-20459100
2024-02-25T18:41:31.222015Z  INFO ThreadId(01) 🎊  shielded-expedition.88f17d1d14 => OpenAckChannel(OpenAck { port_id: transfer, channel_id: channel-440, connection_id: connection-670, counterparty_port_id: transfer, counterparty_channel_id: channel-3878 }) at height 0-65905
2024-02-25T18:41:49.423698Z  INFO ThreadId(01) 🎊  theta-testnet-001 => OpenConfirmChannel(OpenConfirm { port_id: transfer, channel_id: channel-3878, connection_id: connection-3381, counterparty_port_id: transfer, counterparty_channel_id: channel-440 }) at height 0-20459110
2024-02-25T18:41:55.637757Z  INFO ThreadId(01) channel handshake already finished for Channel { ordering: ORDER_UNORDERED, a_side: ChannelSide { chain: BaseChainHandle { chain_id: shielded-expedition.88f17d1d14 }, client_id: 07-tendermint-1557, connection_id: connection-670, port_id: transfer, channel_id: channel-440, version: None }, b_side: ChannelSide { chain: BaseChainHandle { chain_id: theta-testnet-001 }, client_id: 07-tendermint-3202, connection_id: connection-3381, port_id: transfer, channel_id: channel-3878, version: None }, connection_delay: 0ns }
SUCCESS Channel {
    ordering: Unordered,
    a_side: ChannelSide {
        chain: BaseChainHandle {
            chain_id: ChainId {
                id: "shielded-expedition.88f17d1d14",
                version: 0,
            },
            runtime_sender: Sender { .. },
        },
        client_id: ClientId(
            "07-tendermint-1557",
        ),
        connection_id: ConnectionId(
            "connection-670",
        ),
        port_id: PortId(
            "transfer",
        ),
        channel_id: Some(
            ChannelId(
                "channel-440",
            ),
        ),
        version: None,
    },
    b_side: ChannelSide {
        chain: BaseChainHandle {
            chain_id: ChainId {
                id: "theta-testnet-001",
                version: 0,
            },
            runtime_sender: Sender { .. },
        },
        client_id: ClientId(
            "07-tendermint-3202",
        ),
        connection_id: ConnectionId(
            "connection-3381",
        ),
        port_id: PortId(
            "transfer",
        ),
        channel_id: Some(
            ChannelId(
                "channel-3878",
            ),
        ),
        version: None,
    },
    connection_delay: 0ns,
}
```
