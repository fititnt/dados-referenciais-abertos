**Rotina paga gerar arquivo(s)**

`topojson ../shapefile/Munic.shp -o municipio.json --id-property=+GEOCODIGO --p name=NOME,uf=UF,codigo=+GEOCODIGO,regiao=REGIAO,meso=MESOREGIAO,micro=MICROREGIA`

`topojson ../shapefile/Munic.shp -o municipio.min-q1000s6.json --id-property=+GEOCODIGO --p n=NOME -q 1000 -s 1e-6`

`topojson ../shapefile/Munic.shp -o municipio.min-sn-q250.json --id-property=+GEOCODIGO -q 250`

**Outros testes**

`topojson ../shapefile/Munic.shp -o municipio.min-q1000.json --id-property=+GEOCODIGO --p n=NOME -q 1000`

`topojson ../shapefile/Munic.shp -o municipio.min-q1000b.json --id-property=+GEOCODIGO -q 1000` # Remove o nome

`topojson ../shapefile/Munic.shp -o municipio.min-q200.json --id-property=+GEOCODIGO --p name=NOME,uf=UF -q 200`

`topojson ../shapefile/Munic.shp -o municipio.min-q200s1e-8.json --id-property=+GEOCODIGO --p name=NOME,uf=UF -q 200 -s 1e-8`

`topojson ../shapefile/Munic.shp -o municipio.min2-q200s1e-8.json --id-property=+GEOCODIGO --p name=NOME -q 200`