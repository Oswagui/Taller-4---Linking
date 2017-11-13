#GENERACION DE TABLAS CON READELF

Se uso el comando readelf para generar las tablas. Se ejecuto las siguientes lineas en la carpeta obj.<br>

- main2.o -> readelf -h main2.o > ../../tablas/main2_table.txt
- addvec.o -> readelf -h addvec.o > ../../tablas/addvec_table.txt
- multvec.o -> readelf -h multvec.o > ../../tablas/multvec_table.txt
