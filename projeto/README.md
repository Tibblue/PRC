# Projeto de PRC

## Como executar
1. Iniciar o GraphDB
    1. Criar um repositorio com o nome "projetoBeta"
    2. Importar o ficheiro ["povoamento.ttl"](https://github.com/Tibblue/PRC/blob/master/projeto/povoamento.ttl) neste repositorio
    3. GraphDB check :heavy_check_mark:
2. Iniciar o JSON-Server (user db)
    1. Abrir terminal e entrar na diretoria ["usersdb"](https://github.com/Tibblue/PRC/tree/master/projeto/usersdb)
    2. Executar `npm install`
    3. Executar `npm run json:server` e deixar a correr
    4. JSON-Server check :heavy_check_mark:
2. Iniciar o NodeJS (back-end)
    1. Abrir terminal e entrar na diretoria ["backend"](https://github.com/Tibblue/PRC/tree/master/projeto/backend)
    2. Executar `npm install`
    3. Executar `npm start` e deixar a correr
    4. NodeJS check :heavy_check_mark:
3. Iniciar o Vue (front-end)
    1. Abrir terminal e entrar na diretoria ["frontend"](https://github.com/Tibblue/PRC/tree/master/projeto/frontend)
    2. Instalar o Vue com npm `npm install -g @vue/cli`
    2. Executar `npm install`
    3. Executar `npm run serve` e deixar a correr
    4. Vue check :heavy_check_mark:

## Ficheiros

* [ontologia.ttl](https://github.com/Tibblue/PRC/blob/master/projeto/ontologia.ttl) - Ontologia criada para o projeto. Como breve introdução, esta ontologia contem as classes Anime, Person e Network.  
* [csv2ttl.py](https://github.com/Tibblue/PRC/blob/master/projeto/csv2ttl.py) - Script Python que recebeu um [dataset da dbpedia em CSV](http://web.informatik.uni-mannheim.de/DBpediaAsTables/DBpedia-en-2016-04/csv/) e gerou individuals para a ontologia criada. Este script cria um ficheiro ["povoamento.ttl"](https://github.com/Tibblue/PRC/blob/master/projeto/povoamento.ttl) que contem os individuals gerados e a ontologia, sendo por isso possivel carrega-lo imediatamente no GraphDB
* [povoamento.ttl](https://github.com/Tibblue/PRC/blob/master/projeto/povoamento.ttl) - Ontologia + Individuals. Pode ser carregado no GraphDB.
* [datasets](https://github.com/Tibblue/PRC/blob/master/projeto/datasets/) - Pasta que contem os CSVs utilizados.
* [userdb](https://github.com/Tibblue/PRC/blob/master/projeto/userdb/) - Pasta que contem o json-server com a informação dos perfis de utilizador.
* [backend](https://github.com/Tibblue/PRC/blob/master/projeto/backend/) - Pasta que contem o servidor NodeJS.
* [frontend](https://github.com/Tibblue/PRC/blob/master/projeto/frontend/) - Pasta que contem o servidor Vue.
