# Pesetacoin Core [PTC] 0.9.2
==========================
PesetaCoin integration/staging tree
================================

http://www.pesetacoin.info

Copyright (c) 2009-2013 Bitcoin Developers<br />
Copyright (c) 2011-2013 Litecoin Developers<br />
Copyright (c) 2014-2018 PesetaCoin Developers


Que es PesetaCoin?
----------------
ESPECIFICACIONES

- Algoritmo Scrypt (POW)
- Número total de monedas: 166,386,000 PTCs 
- 166(.386) monedas por bloque (nueva tabla de recompensas)
- Block target: 1 minuto 
- Con soporte para Merged Mining
- RPC Port: 16638
- P2P Port: 16639

Recompensa
----------------------------------

    0 - 525,599:          166.386 PTC
    525,599 - 549,999:     83.193 PTC
    550,000 - 1,051,199:   50 PTC
    1,051,200 - 1,576,799: 25 PTC
    1,576,800 - 2,627,999: 10 PTC
    2,628,000 - 8,409,599:  5 PTC
    8,409,600+: 0 PTC
    
Compilación sin entorno gráfico:
----------------------------------

 
Instalar dependencias, clonar repositorio y compilar: 

	sudo apt-get update
	sudo apt-get install autoconf
	sudo apt-get install software-properties-common
	sudo add-apt-repository ppa:bitcoin/bitcoin y enter
	sudo apt-get update
	sudo apt-get install libdb5.3-dev libdb5.3++-dev
	sudo apt-get install libboost-all-dev
	sudo apt-get install libssl-dev
	sudo apt-get install libprotobuf-dev
	sudo apt install protobuf-compiler
	sudo apt-get install libqt4-dev
	git clone https://github.com/FundacionPesetacoin/Pesetacoin-0.9.2-Oficial.git
	cd Pesetacoin-0.9.2-Oficial/
	./autogen.sh
	./configure --with-incompatible-bdb
	make -j 4
 
	

Compilación con entorno gráfico:
----------------------------------

Es necesario tener las librerias anteriormente mencionadas instaladas.

Ejecutar:

	./autogen.sh
	./configure --with-incompatible-bdb --with-gui=qt4
	make -j 4


License
-------

PesetaCoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Pesetacoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion (if they haven't already) on the
[mailing list](http://sourceforge.net/mailarchive/forum.php?forum_name=bitcoin-development).

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoin/bitcoin/tags) are created
regularly to indicate new official, stable release versions of Pesetacoin.


