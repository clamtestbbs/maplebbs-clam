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

SBBS = $(SRCD)/sample/bbs

SCON = $(SRCD)/sample/config.h

#SMAK = ../src        ## not done yet

all: 
	@echo "Please enter 'make sample-type', "
	@echo " make init   : for install sample BBS structure (cover old data) "
	@echo " make config : for install sample config for a new BBS (still need correct manually)"

init:
	@cp -r $(SBBS)/* ~/;cp $(SBBS)/.BRD ~/
	@cp $(SCON) ../src/include/
	@crontab ./crontab

config:
	@cp $(SCON) ../src/include/

#mainmake:            ## not done yet

