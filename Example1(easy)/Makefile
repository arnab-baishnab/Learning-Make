# Name of the binary
BINARY_NAME=myapp

# Directory to store the compiled binary
BUILD_DIR=bin

# Default target
all: build

# Build the binary
build:
	@echo "Building the binary..."
	@mkdir -p $(BUILD_DIR)
	@go build -o $(BUILD_DIR)/$(BINARY_NAME) main.go

# Clean up build artifacts
clean:
	@echo "Cleaning up..."
	@rm -rf $(BUILD_DIR)

# Run the binary
run: build
	@echo "Running the application..."
	@./$(BUILD_DIR)/$(BINARY_NAME)

# Default behavior: build and run
.PHONY: all build clean run
