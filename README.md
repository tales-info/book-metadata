Endpoints de busca
=========================

Pesquisa
-------------------------
Formato:

/search/:termo-de-busca?start=0&format=json

:termo-de-busca: pode ser o nome de um livro, autor, etc..
start: por padrão o valor é 0. serve para paginar o resultado
format: por padrão é json. mas pode ser setado como xml

Endpoints:

 - http://177.44.76.41:5000/search/ziviani
 - http://177.44.76.41:5000/search/ziviani?start=10
 - http://177.44.76.41:5000/search/ziviani?start=20&format=xml

Obter pelo isbn
-------------------------
Formato:

/get/:isbn1/:isbn2/...&format=json

:isbn1, isbn2,... : um ou mais isbn para retornar (isbn 10 ou isbn 13)
format: por padrão é json. mas pode ser setado como xml

Endpoints:

 - http://177.44.76.41:5000/get/1849051259
 - http://177.44.76.41:5000/get/9781568823522
 - http://177.44.76.41:5000/get/1849051259/9781568823522
 - http://177.44.76.41:5000/get/1849051259/9781568823522&format=xml
