Name:                   Veles (Cryptomoneda)
Image:                  /images/logo/veles256.png
Ticker:                 VLS
ProgrammingLanguage:    C++
InitialRelease:         Noviembre 2018
OrgStructure:           Decentralized
OpenSource:             Si
License:                MIT
ConsensusMechanism:     Proof of Work
DevelopmentStatus:      Alpha (activo)
Bitcointalk:            [\[ANN\] ▼ VELES ... ](https://bitcointalk.org/index.php?topic=5064523)
Website:                https://www.veles.network/index.es.html
Whitepaper:             [WP - First Release](https://veles.network/Whitepaper.wiki.es.html)

# Especificaciones de la Moneda

Especificaciones Generales  | :
----------------------- | -------------------------------------------
Algoritmos de minado    | Lyra2z, X11, X16R, Sha256d, Scrypt, Nist5
Unidades Máximas        | 2 500 000 VLS
Unidades en Circulación | {: data-entity-id="market.price" data-attribute="total_supply" data-format="number" data-fixed-decimals="2" data-unit="VLS" .ws }
Tiempo de Bloque        | 2 minutos 
Preminado (swap)        | 50 000 VLS
Bloques actualmente     | {: data-entity-id="chain.tip" data-format="number" data-attribute="height" data-unit="blocks" .ws }

Especificaciones Masternode | :
--------------------------- | ---------------------------------------
Colateral de Masternode     | 500 VLS
Número de Masternodes       | {: data-entity-id="masternodes" data-attribute="count" .ws }
dApps en ejecución          | dVPN, dDNS (recursive)

Especificaciones de recompensa de Bloques | ⚒
----------------------------------------- | ---------------------------------------
Recompensa Máxima por Bloque              | {: data-entity-id="chain.halving.status" data-attribute="max_block_reward" data-format="number" data-fixed-decimals="2" data-unit="VLS" .ws }
Recompensa Mínima por Bloque              | 0.01 VLS
Recompensa Promedio por Bloque            | {: data-entity-id="chain.stats.mining" data-attribute="block_reward_average" data-format="number" data-fixed-decimals="2" data-unit="VLS" .ws }
Recompensa por minado PoW %               | {: data-entity-id="chain.stats.mining" data-attribute="block_reward_pow_percent" data-format="number" data-fixed-decimals="2" data-unit="%" .ws }
Recompensa para Masternode %              | {: data-entity-id="chain.stats.mining" data-attribute="block_reward_mn_percent" data-format="number" data-fixed-decimals="2" data-unit="%" .ws }
Recompensa para Dev Team %                | {: data-entity-id="chain.stats.mining" data-attribute="block_reward_dev_percent" data-format="number" data-fixed-decimals="2" data-unit="%" .ws }
Billetera Dev Team                        | VKtig9w7wfx6Ep9B4NnbwxLj1bkY2kHXBj

Halving de recompensa por Bloque  | ⚒
--------------------------------- | ------------------------------------
Bloques hasta siguiente Halving:  | {: .chain-pow-blocks-to-next-epoch .ws }
Bloque de Inicio de Epoch         | {: data-entity-id="chain.halving.status" data-attribute="start_block" .ws }
Bloque de fin de Epoch            | {: data-entity-id="chain.halving.status" data-attribute="end_block" .ws }
Unidades emitidas desde Halving   | {: data-entity-id="chain.halving.status" data-attribute="supply_since_halving" data-format="number" data-fixed-decimals="2" data-unit="VLS" .ws }
Objetivo de Emisión               | 160 000 VLS
Porcentaje alcanzado actual       | {: data-entity-id="chain.halving.status" data-attribute="supply_target_reached" .ws }
Porcentaje mínimo requerido       | 80%
Epoch actual                      | {: data-entity-id="chain.halving.status" data-attribute="epoch_name" .ws }


Para más información y una lista completa de los Halvings anteriores vea la página [Halving Epochs table on the Mining Stats](https://explorer.veles.network/miningstats#halving-epoch-table) en el Explorador. También puede utilizar el comando `gethalvingstatus` en su billetera local. 


!!! note ""
    Items  mostrados en verde se cambian dinámicamente por el mecanismo de consenso de la red y muestran valores actualizados.
    {: .ws}

    Si algunos valores no se muestran es probable que sea debido a que no está viendo esta página utilizando la web-app oficial de la wiki.
    De ser así por favor visita
    [current page on the Veles Core wiki](http://veles.network/Coin-Specifications.wiki.en.html).
    Si ya es así entonces tu navegador está teniendo problemas para conectarse con el servidor.
    {: .websocket-offline}
