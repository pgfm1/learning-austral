BIN := "program"

MODULES := \
		   ../standard/Tuples.aui,../standard/Tuples.aum \
		   ../standard/Bounded.aui,../standard/Bounded.aum \
		   ../standard/Equality.aui,../standard/Equality.aum \
		   ../standard/Order.aui,../standard/Order.aum \
		   ../standard/Box.aui,../standard/Box.aum \
		   ../standard/Buffer.aui,../standard/Buffer.aum \
		   ../standard/String.aui,../standard/String.aum \
		   ../standard/StringBuilder.aui,../standard/StringBuilder.aum \
		   ../standard/IO/IO.aui,../standard/IO/IO.aum \
		   ../standard/IO/Terminal.aui,../standard/IO/Terminal.aum \
		   Stack.aui,Stack.aum \
		   Main.aum

.DEFAULT: all

all: $(BIN)

$(BIN): ../standard/*.aui ../standard/*.aum ../standard/IO/*.aui ../standard/IO/*.aum *.aui *.aum
	austral compile $(MODULES) --entrypoint=Main:main --output=$(BIN)

.PHONY: clean
clean:
	@rm $(BIN) 2> /dev/null || true
