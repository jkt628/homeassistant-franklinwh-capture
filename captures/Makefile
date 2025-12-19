SRCS := $(wildcard *.har)
OBJS := $(SRCS:.har=.json)
.PHONY: FORCE

%.json: %.har
	../.venv/bin/python ../bin/sanitize $< > $@
$(OBJS): FORCE
