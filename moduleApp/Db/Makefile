TOP = ../..
include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE

#----------------------------------------------------
#  Optimization of db files using dbst (DEFAULT: NO)
#DB_OPT = YES

#----------------------------------------------------
# Create and install (or just install) dbd files
# <name>.dbd will be created from <name>Include.dbd
#DBD += example.dbd

#----------------------------------------------------
# Create and install (or just install)
# databases, templates, substitutions like this
#DB += softMotorexample.db

DB += $(patsubst ../%, %, $(wildcard ../*.template))
DB += $(patsubst ../%, %, $(wildcard ../*.db))
DB += $(patsubst ../%, %, $(wildcard ../*.vdb))

DB += $(patsubst ../%, %, $(wildcard ../*.proto))
DB += $(patsubst ../%, %, $(wildcard ../*.protocol))

REQ += $(patsubst ../%, %, $(wildcard ../*.req))

#----------------------------------------------------
# Declare template files which do not show up in DB
#USES_TEMPLATE += dbExample2.template

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE
