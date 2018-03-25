# This is the master test runner
# This will execute every test file named *.test in this directory

TEST_FILES := $(wildcard *.test)
PASS_FILES := $(patsubst %.test, %.pass, $(TEST_FILES) )

ifndef VERBOSE
.SILENT:
endif

__default: $(PASS_FILES)

all: __default
	#

%.pass : %.test
	# Attempting to run: $<
	[ -x $< ] && ( $< || echo FAIL: $< ) && echo PASS: $< 
