# preserv-BO
[Preservación digital](https://en.wikipedia.org/wiki/Digital_preservation) de las principales fuentes de la **base de datos AddressForAll-Bolivia**, mantenida por el [Instituto AddressForAll](http://addressforall.org/).

A Bolivia se le asignó: en el contexto [ISO&nbsp;3166](https://en.wikipedia.org/wiki/ISO_3166) el geocódigo [**BO**](https://en.wikipedia.org/wiki/ISO_3166-2:BO) y el número [**68**](https://en.wikipedia.org/wiki/ISO_3166-1_numeric); en [Wikidata](https://wikidata.org) el identificador [Q750](http://wikidata.org/entity/Q750); en [OpenStreetMap](https://osm.org) el identificador de [*relación* 252645](http://osm.org/relation/252645).


## Organización territorial


## Organización de este repositorio

En este *git*, **solo se guardan los metadatos**, es decir, descriptores de entidad, como nombres y códigos geográficos &mdash; mapas y otros datos brutos, almacenados externamente porque son muy grandes.  Posteriormente, los "datos en bruto", no estandarizados, se convierten en "datos filtrados" y se conservan en lo [*git* preservCutGeo‑BO2021](http://git.digital-guard.org/preservCutGeo-BO2021).

Los metadatos se organizaron de la siguiente manera, en la carpeta [`/data`](./data):

* [`/data`](./data): "datos", todos los metadatos originales de **entrada**, es decir, metadatos proporcionados para el sistema.
   * `jurisdictionLevel*.csv`:  jurisdicciones (en todos los niveles) y sus geocódigos. La primera subdivisión es [jurisdictionLevel4.csv](./data/jurisdictionLevel4.csv).
   * [`donor.csv`](./data/donor.csv): donantes de paquetes de datos. Metadatos de las instituciones que brindan datos oficiales. (pendente)
   * [`donatedPack.csv`](./data/donatedPack.csv): descriptores de los archivos donados. (pendente)
   * *paquetes* (carpetas `_packXX`): *hash*  y otros descriptores de archivos almacenados externamente, así como `makefile` y otros descriptores de proceso para descomprimir estos archivos y llevarlos a la base de datos (PostregSQL)... 

* [`/data/_out`](./data/out): resultados generados por el sistema (**salida**), es decir, metadatos creados a partir de los algoritmos y estadísticas aplicados a los datos de `_pack`.

* [`/src`](./src#readme): reservado a código fuente de algoritmos SQL, *makefile* y otros de uso local. Ver código fuente general em [Preserv](http://git.digital-guard.org/preserv).

## Licencia
[Licencia CC0](https://creativecommons.org/publicdomain/zero/1.0/deed.es).
