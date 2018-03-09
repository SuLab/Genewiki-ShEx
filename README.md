# genewiki Shape Expressions. 
## Shapes
| Shape | Jenkins | Jupyter | shex.js | Shaclex | 
|---|---|---|---|---|
|genes  |-|[+](https://colab.research.google.com/drive/1QSXPdEL77V13d93XmWO5K5-TQTIYS_P7#scrollTo=Mkd5GKBOdueV)|[+](https://rawgit.com/shexSpec/shex.js/wikidata/doc/shex-simple.html?manifestURL=https://raw.githubusercontent.com/SuLab/Genewiki-ShEx/master/genes/manifest.json) |[+](http://shaclex.herokuapp.com/load?manifestURL=https://raw.githubusercontent.com/SuLab/Genewiki-ShEx/master/genes/manifest.json)|
| proteins  |-|-|[+](https://rawgit.com/shexSpec/shex.js/wikidata/doc/shex-simple.html?manifestURL=https://raw.githubusercontent.com/SuLab/Genewiki-ShEx/master/proteins/manifest.json)| [+](http://shaclex.herokuapp.com/load?manifestURL=ttps://raw.githubusercontent.com/SuLab/Genewiki-ShEx/master/proteins/manifest.json)|
| diseases  |-|-|[+](https://rawgit.com/shexSpec/shex.js/wikidata/doc/shex-simple.html?manifestURL=https://raw.githubusercontent.com/SuLab/Genewiki-ShEx/master/diseases/manifest.json)|[+](http://shaclex.herokuapp.com/load?manifestURL=ttps://raw.githubusercontent.com/SuLab/Genewiki-ShEx/master/diseases/manifest.json)|
| pathways (wikipathways) |-|[+](https://colab.research.google.com/drive/10hUMlUlKyApJEXQ0XGxd7U9GZ9WSWGxL#scrollTo=Mkd5GKBOdueV)|[+](https://rawgit.com/shexSpec/shex.js/wikidata/doc/shex-simple.html?manifestURL=https://raw.githubusercontent.com/SuLab/Genewiki-ShEx/master/pathways/wikipathways/manifest.json)|[+](http://shaclex.herokuapp.com/load?manifestURL=ttps://raw.githubusercontent.com/SuLab/Genewiki-ShEx/master/pathways/wikipathways/manifest.json)|
| pathway (reactome) |-|[+](https://colab.research.google.com/drive/1bWxsXuv04eq1ozn9z9MJ7Xlu2meQ5R1c#scrollTo=Mkd5GKBOdueV&line=12&uniqifier=1)|[+](https://rawgit.com/shexSpec/shex.js/wikidata/doc/shex-simple.html?manifestURL=https://raw.githubusercontent.com/shexSpec/schemas/master/Wikidata/pathways/Reactome/manifest.json)|[+](http://shaclex.herokuapp.com/load?manifestURL=ttps://raw.githubusercontent.com/SuLab/Genewiki-ShEx/master/Reactome/manifest.json)|
| variants  |-|-|-|-|


This repository collects Shape Expression to model and validate Wikidata items added by bots developed and maintained in the Gene wiki project. 
## Installation
Running Shape expressions requires shex.js. Installation instructions can be found [here](https://github.com/shexSpec/shex.js/)
## Usage
With shex.js running the following commands downloads the shapes collected here and run them against a select set of on topic items. 
### Human gene
```
./bin/validate -x https://raw.githubusercontent.com/shexSpec/schemas/master/Wikidata/genewiki/wikidata_human-genes.shex -d https://www.wikidata.org/wiki/Special:EntityData/Q17853226.ttl

``` 

### Disease
```
./bin/validate -x https://raw.githubusercontent.com/shexSpec/schemas/master/Wikidata/genewiki/wikidata_disease.shex -d https://www.wikidata.org/wiki/Special:EntityData/Q35869.ttl -s wikidata-disease -n http://www.wikidata.org/entity/Q35869
``` 

### CIViC variant
``` 
.//Users/andra/bin/validate -x https://raw.githubusercontent.com/shexSpec/schemas/master/Wikidata/genewiki/wikidata-civic.shex -d https://www.wikidata.org/wiki/Special:EntityData/Q21851559.ttl -s wikidata-civic_variant_record -n http://www.wikidata.org/entity/Q21851559
```
## Contributing
1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D





