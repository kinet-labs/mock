# mock
Mock utilities and testing helpers

## Features

- **GoMock utilities**: Simplified gomock controller and matcher utilities
- **Mock generators**: Tools for generating mocks
- **Test helpers**: Common testing utilities

## Installation

```bash
go get github.com/kinet-labs/mock
```

## Usage

```go
import (
    "github.com/kinet-labs/mock/gomock"
)

func TestExample(t *testing.T) {
    ctrl := gomock.NewController(t)
    defer ctrl.Finish()
    
    // Use your mocks here
}
```

## Generating Mocks

Use the standard mockgen tool:

```bash
mockgen -source=interface.go -destination=mocks/mock_interface.go -package=mocks
```