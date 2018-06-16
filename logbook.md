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

```