# When building consider using the following options:
#
CURRENT_TIME=$(shell python ./timeSec.py) #Set the time on the clock to current time. no ntp means you need a good starting point

COMPONENT=JustFATLoggingC

ifdef CURRENT_TIME
PFLAGS += -DCURRENT_TIME=$(CURRENT_TIME)
endif

# this tells the sd driver to use proper clock calibration for spi bus during card init
PFLAGS += -DSMCLK_4MHZ

include $(MAKERULES)
