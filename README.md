# time_series_trading
Contrairement à l'idée répandue chez les datascientists non-initiés à la finance de marché, il est assez difficile de prédire l'orientation des prix d'un actif financier par extrapolation en se basant uniquement sur ses prix (Open/Close/High/Low), ou sur des indicateurs techniques qui en dérivent.

Tout d'abord, il est important de comprendre que les professionnels de la finance de marché ne font pas de prévision sur l'orientation des prix. Ils recherchent des patterns, c'est-à-dire des schémas, des configurations récurrentes qui offrent un avantage statistique lorsqu'ils sont utilisés un grand nombre de fois.

Ces schémas sont difficilement identifiables en analysant uniquement les prix. Les traders discrétionnaires des firms de proprietary trading utilisent des patterns qui se basent sur le temps, le prix et le volume. Les traders quantitatifs de ces mêmes firmes peuvent utiliser en plus de ce triptyque temps/prix/volume, des données quantitatives (ex: données 3 de l'order flow...), fondamentales (ex : taux d'intérêt de la FED, NFP...) et alternatives (utilisation de NLP ou de computer vision pour capturer le sentiment des investisseurs, des image satellites...)

Dans ce projet, nous allons créer un modèle qui utilise des données basées sur le triptyque temps/prix/volumes. Nous allons ensuite backtester notre modèle, puis nous le mettrons en production sur un serveur AWS en utilisant une API qui permet de se connecter au futures du CME et faire du trading live.
