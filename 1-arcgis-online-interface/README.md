#tutorial02: planejar rotas para entregadores de mercadorias

Para planejar as rotas dos seus cinco entregadores, você precisará de três camadas: uma para os pontos de partida (o Centro de Distribuição do Mercado Livre), uma para os destinos de entrega (os 23 endereços de clientes) e outro para os pontos de chegada final (as residências de cada entregador). Essas duas últimas camadas serão criadas a partir de arquivos CSV (valores separados por vírgulas), em que cada linha representa um registro (endereço do cliente ou residência) e cada campo separa os atributos das feições.

Os endereços contidos nos arquivos CSV podem ser geocodificados em um mapa no ArcGIS Online. A geocodificação é uma operação de SIG que converte endereços em dados espaciais para que possam ser mapeados.

Você fará o download de dois arquivos CSV e os usará para geocodificar os endereços no seu mapa: um contendo os endereços dos 23 destinos que sua equipe irá realizar as entregas e outro com os endereços das residências dos entregadores.
