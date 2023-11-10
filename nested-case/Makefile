BIN := "program"

MODULES := Main.aum

.DEFAULT: all

all: $(BIN)

$(BIN): Main.aum
	austral compile $(MODULES) --entrypoint=Main:main --output=$(BIN)

run: $(BIN)
	@./program

.PHONY: clean
clean:
	@rm $(BIN) 2> /dev/null || true
