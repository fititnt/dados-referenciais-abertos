# Diário de bordo - Eventos informantes
Arquivo meramente para listar comandos usados

```bash
 fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [15:17:25]
$ wget ftp://geoftp.ibge.gov.br/organizacao_do_territorio/malhas_territoriais/malhas_municipais/municipio_2016/Brasil/BR/BR.zip
--2018-06-16 15:20:11--  ftp://geoftp.ibge.gov.br/organizacao_do_territorio/malhas_territoriais/malhas_municipais/municipio_2016/Brasil/BR/BR.zip
           => “BR.zip”
Resolvendo geoftp.ibge.gov.br (geoftp.ibge.gov.br)... 186.228.51.6
Conectando-se a geoftp.ibge.gov.br (geoftp.ibge.gov.br)|186.228.51.6|:21... conectado.
Acessando como anonymous ... Acesso autorizado!
==> SYST ... feito.    ==> PWD ... feito.
==> TYPE I ... feito.  ==> CWD (1) /organizacao_do_territorio/malhas_territoriais/malhas_municipais/municipio_2016/Brasil/BR ... feito.
==> SIZE BR.zip ... 167304811
==> PASV ... feito.    ==> RETR BR.zip ... feito.
Tamanho: 167304811 (160M) (não autoritário)

BR.zip                       100%[=============================================>] 159,55M   647KB/s    in 4m 10s  

2018-06-16 15:24:21 (652 KB/s) - “BR.zip” salvo [167304811]

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [15:24:22]
$ mv BR.zip temp 

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [15:28:23]
$ unzip temp/BR.zip -d temp/BR

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [15:29:05]
$ unzip temp/BR.zip -d temp/  
Archive:  temp/BR.zip
   creating: temp/BR/
 extracting: temp/BR/BRMEE250GC_SIR.cpg  
  inflating: temp/BR/BRMEE250GC_SIR.dbf  
  inflating: temp/BR/BRMEE250GC_SIR.prj  
  inflating: temp/BR/BRMEE250GC_SIR.shp  
  inflating: temp/BR/BRMEE250GC_SIR.shx  
 extracting: temp/BR/BRMIE250GC_SIR.cpg  
  inflating: temp/BR/BRMIE250GC_SIR.dbf  
  inflating: temp/BR/BRMIE250GC_SIR.prj  
  inflating: temp/BR/BRMIE250GC_SIR.shp  
  inflating: temp/BR/BRMIE250GC_SIR.shx  
 extracting: temp/BR/BRMUE250GC_SIR.cpg  
  inflating: temp/BR/BRMUE250GC_SIR.dbf  
  inflating: temp/BR/BRMUE250GC_SIR.prj  
  inflating: temp/BR/BRMUE250GC_SIR.shp  
  inflating: temp/BR/BRMUE250GC_SIR.shx  
 extracting: temp/BR/BRUFE250GC_SIR.cpg  
  inflating: temp/BR/BRUFE250GC_SIR.dbf  
  inflating: temp/BR/BRUFE250GC_SIR.prj  
  inflating: temp/BR/BRUFE250GC_SIR.shp  
  inflating: temp/BR/BRUFE250GC_SIR.shx 

$ ls -lha temp/BR
total 223M
drwxrwxr-x 2 fititnt fititnt 4,0K Jun 23  2017 .
drwxrwxr-x 3 fititnt fititnt 4,0K Jun 16 15:29 ..
-rw-rw-r-- 1 fititnt fititnt    5 Jun 23  2017 BRMEE250GC_SIR.cpg
-rw-rw-r-- 1 fititnt fititnt  15K Jun 23  2017 BRMEE250GC_SIR.dbf
-rw-rw-r-- 1 fititnt fititnt  151 Jun 23  2017 BRMEE250GC_SIR.prj
-rw-rw-r-- 1 fititnt fititnt  26M Jun 23  2017 BRMEE250GC_SIR.shp
-rw-rw-r-- 1 fititnt fititnt 1,2K Jun 23  2017 BRMEE250GC_SIR.shx
-rw-rw-r-- 1 fititnt fititnt    5 Jun 23  2017 BRMIE250GC_SIR.cpg
-rw-rw-r-- 1 fititnt fititnt  58K Jun 23  2017 BRMIE250GC_SIR.dbf
-rw-rw-r-- 1 fititnt fititnt  151 Jun 23  2017 BRMIE250GC_SIR.prj
-rw-rw-r-- 1 fititnt fititnt  50M Jun 23  2017 BRMIE250GC_SIR.shp
-rw-rw-r-- 1 fititnt fititnt 4,5K Jun 23  2017 BRMIE250GC_SIR.shx
-rw-rw-r-- 1 fititnt fititnt    5 Jun 23  2017 BRMUE250GC_SIR.cpg
-rw-rw-r-- 1 fititnt fititnt 371K Jun 23  2017 BRMUE250GC_SIR.dbf
-rw-rw-r-- 1 fititnt fititnt  151 Jun 23  2017 BRMUE250GC_SIR.prj
-rw-rw-r-- 1 fititnt fititnt 137M Jun 23  2017 BRMUE250GC_SIR.shp
-rw-rw-r-- 1 fititnt fititnt  44K Jun 23  2017 BRMUE250GC_SIR.shx
-rw-rw-r-- 1 fititnt fititnt    5 Jun 23  2017 BRUFE250GC_SIR.cpg
-rw-rw-r-- 1 fititnt fititnt 2,1K Jun 23  2017 BRUFE250GC_SIR.dbf
-rw-rw-r-- 1 fititnt fititnt  151 Jun 23  2017 BRUFE250GC_SIR.prj
-rw-rw-r-- 1 fititnt fititnt 8,9M Jun 23  2017 BRUFE250GC_SIR.shp
-rw-rw-r-- 1 fititnt fititnt  316 Jun 23  2017 BRUFE250GC_SIR.shx

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [15:35:03]
$ mkdir -p {uf,mesorregiao,microrregiao,municipio}/shapefile/2018/

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [15:36:33]
$ touch {uf,mesorregiao,microrregiao,municipio}/shapefile/2018/README.md


# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 o [15:40:10]
$ cp temp/BR/BRMUE250GC_SIR* municipio/shapefile/2018/

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [15:41:51]
$ cp temp/BR/BRMIE250GC* microrregiao/shapefile/2018/

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [15:43:33]
$ cp temp/BR/BRMEE250GC* mesorregiao/shapefile/2018/

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [15:44:26]
$ cp temp/BR/BRUFE250GC* uf/shapefile/2018/

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [15:44:59]
$ echo -e "# The .shp are too big to commit. We will commit compressed 7z \n*.shp" > {uf,mesorregiao,microrregiao,municipio}/shapefile/2018/.gitignore 

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [16:03:23]
$ cd /alligo/code/fititnt/gis-dataset-brasil/uf/shapefile/2018

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil/uf/shapefile/2018 on git:atualizacao-jun-2018 x [16:05:25]
$ 7z a BRUFE250GC_SIR.shp.7z BRUFE250GC_SIR.shp

7-Zip [64] 9.20  Copyright (c) 1999-2010 Igor Pavlov  2010-11-18
p7zip Version 9.20 (locale=pt_BR.UTF-8,Utf16=on,HugeFiles=on,8 CPUs)
Scanning

Creating archive BRUFE250GC_SIR.shp.7z

Compressing  BRUFE250GC_SIR.shp      

Everything is Ok

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil/mesorregiao/shapefile/2018 on git:atualizacao-jun-2018 x [16:06:19]
$ 7z a BRMEE250GC_SIR.shp.7z BRMEE250GC_SIR.shp

7-Zip [64] 9.20  Copyright (c) 1999-2010 Igor Pavlov  2010-11-18
p7zip Version 9.20 (locale=pt_BR.UTF-8,Utf16=on,HugeFiles=on,8 CPUs)
Scanning

Creating archive BRMEE250GC_SIR.shp.7z

Compressing  BRMEE250GC_SIR.shp      

Everything is Ok

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil/mesorregiao/shapefile/2018 on git:atualizacao-jun-2018 x [16:06:42]
$ cd /alligo/code/fititnt/gis-dataset-brasil/microrregiao/shapefile/2018

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil/microrregiao/shapefile/2018 on git:atualizacao-jun-2018 x [16:07:50]
$ 7z a BRMIE250GC_SIR.shp.7z BRMIE250GC_SIR.shp

7-Zip [64] 9.20  Copyright (c) 1999-2010 Igor Pavlov  2010-11-18
p7zip Version 9.20 (locale=pt_BR.UTF-8,Utf16=on,HugeFiles=on,8 CPUs)
Scanning

Creating archive BRMIE250GC_SIR.shp.7z

Compressing  BRMIE250GC_SIR.shp      

Everything is Ok

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil/microrregiao/shapefile/2018 on git:atualizacao-jun-2018 x [16:08:47]
$ cd /alligo/code/fititnt/gis-dataset-brasil/municipio/shapefile/2018

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil/municipio/shapefile/2018 on git:atualizacao-jun-2018 x [16:09:16]
$ 7z a BRMUE250GC_SIR.shp.7z BRMUE250GC_SIR.shp

7-Zip [64] 9.20  Copyright (c) 1999-2010 Igor Pavlov  2010-11-18
p7zip Version 9.20 (locale=pt_BR.UTF-8,Utf16=on,HugeFiles=on,8 CPUs)
Scanning

Creating archive BRMUE250GC_SIR.shp.7z

Compressing  BRMUE250GC_SIR.shp      

Everything is Ok

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil/municipio/shapefile/2018 on git:atualizacao-jun-2018 x [16:10:49]
$ cd /alligo/code/fititnt/gis-dataset-brasil/

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 o [1:06:54]
$ ogr2ogr -f GeoJSON temp/municipio.json municipio/shapefile/2018/BRMUE250GC_SIR.shp

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 o [1:09:35]
$ ls -lha temp/municipio.json
-rw-rw-r-- 1 fititnt fititnt 362M Jun 19 01:09 temp/municipio.json

# NOTE: PQP 360MB é grande demais pra commitar.

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 o [1:11:29]
$ 7z a temp/municipio.json.7z temp/municipio.json 

7-Zip [64] 9.20  Copyright (c) 1999-2010 Igor Pavlov  2010-11-18
p7zip Version 9.20 (locale=pt_BR.UTF-8,Utf16=on,HugeFiles=on,8 CPUs)
Scanning

Creating archive temp/municipio.json.7z

Compressing  temp/municipio.json      

Everything is Ok

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 o [1:18:20]
$ ls -lha temp/municipio.json.7z                 
-rw-rw-r-- 1 fititnt fititnt 55M Jun 19 01:18 temp/municipio.json.7z

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 o [1:19:09]
$ rm -f municipio/geojson/municipio.json

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [1:30:03]
$ ogr2ogr --version
GDAL 2.1.3, released 2017/20/01

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [1:23:32]
$ 7z a municipio/geojson/municipio.json.7z temp/municipio.json 

7-Zip [64] 9.20  Copyright (c) 1999-2010 Igor Pavlov  2010-11-18
p7zip Version 9.20 (locale=pt_BR.UTF-8,Utf16=on,HugeFiles=on,8 CPUs)
Scanning

Creating archive municipio/geojson/municipio.json.7z

Compressing  temp/municipio.json      

Everything is Ok

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [1:31:17]
$ ogr2ogr -f GeoJSON temp/microrregiao.json microrregiao/shapefile/2018/BRMIE250GC_SIR.shp

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [1:34:10]
$ ls -lha temp/microrregiao.json
-rw-rw-r-- 1 fititnt fititnt 134M Jun 19 01:34 temp/microrregiao.json

## NOTE: ainda é grande (fititnt, 2018-06-19 01:37)

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [1:39:07]
$ rm -f microrregiao/geojson/microrregiao.json

# fititnt at bravo in /alligo/code/fititnt/gis-dataset-brasil on git:atualizacao-jun-2018 x [1:39:40]
$ 7z a microrregiao/geojson/microrregiao.json.7z temp/microrregiao.json

7-Zip [64] 9.20  Copyright (c) 1999-2010 Igor Pavlov  2010-11-18
p7zip Version 9.20 (locale=pt_BR.UTF-8,Utf16=on,HugeFiles=on,8 CPUs)
Scanning

Creating archive microrregiao/geojson/microrregiao.json.7z

Compressing  temp/microrregiao.json      

Everything is Ok

## NOTE: ops, os arquivos do 7z salvam com a pasta. Deletar e refazer  (fititnt, 2018-06-19 01:43)

```