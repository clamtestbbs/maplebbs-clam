# ------------------------------------------------------ #
#  Makefile     ( MapleBBS - WindTop -DreamBBS )         #
# ------------------------------------------------------ #
#  author : r2.bbs@bbs.ccns.ncku.edu.tw                  #
#  target : Makefile for DreamBBS sample files           #
#  create : 2017/08/10                                   #
#  update : 2017/  /                                     #
# ------------------------------------------------------ #


####### CAUTION: Still Testing!! Don't try it on important sites #######

BBSHOME = /home/bbs

SRCD = $(BBSHOME)/maplebbs-clam

SAM  = $(SRCD)/sample

SBBS = $(SAM)/bbs

SCON = $(SAM)/config.h

#SMAK = ../src        ## not done yet

all:
	@echo "Please enter 'make sample-type', "
	@echo -e " make init   : for install sample BBS structure (\033[1;31mWARNING: will COVER old data!!\033[m) "
	@echo " make config : for install sample config for a new BBS (still need correct manually)"

install:
	@echo "Please enter 'make sample-type', "
	@echo -e " make init   : for install sample BBS structure (\033[1;31mWARNING: will COVER old data!!\033[m) "
	@echo " make config : for install sample config for a new BBS (still need correct manually)"


init:
	@cp -ir $(SAM)/bbs/* $(BBSHOME)/ ; cp $(SAM)/bbs/.BRD $(BBSHOME)/
	@cp -i $(SAM)/config.h $(SRCD)/include/
	@vim -c 'set fencs=big5' -c 'e!' $(SRCD)/include/config.h
	@crontab $(SAM)/crontab
	@crontab -e

config:
	@cp -i $(SAM)/config.h $(SRCD)/include/

#mainmake:            ## not done yet

