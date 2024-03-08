<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	speakeasybarsamplesdk "github.com/speakeasy-sdks/speakeasy-bar-sample-sdk"
	"github.com/speakeasy-sdks/speakeasy-bar-sample-sdk/pkg/models/shared"
	"log"
)

func main() {
	s := speakeasybarsamplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx, shared.Pet{
		ID:   596804,
		Name: "<value>",
	})
	if err != nil {
		log.Fatal(err)
	}
	if res != nil {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->