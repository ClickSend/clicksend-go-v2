# ClickSend Go SDK

Official Go client for the [ClickSend API](https://developers.clicksend.com/) — send and manage SMS, MMS, email, voice, fax, letters, postcards, and more.

## Installation

```sh
go get github.com/ClickSend/clicksend-go-v2
```

## Getting Started

```go
package main

import (
	"context"
	"fmt"
	"os"

	clicksend "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	cfg := clicksend.NewConfiguration()
	client := clicksend.NewAPIClient(cfg)

	auth := context.WithValue(context.Background(), clicksend.ContextBasicAuth, clicksend.BasicAuth{
		UserName: os.Getenv("CLICKSEND_USERNAME"),
		Password: os.Getenv("CLICKSEND_API_KEY"),
	})

	smsMessageCollection := clicksend.SmsMessageCollection{
		Messages: []clicksend.SmsMessage{
			{Source: "sdk", Body: "Hello from ClickSend!", To: "+61411111111"},
		},
	}

	result, _, err := client.SMSAPI.SmsSendPost(auth).SmsMessageCollection(smsMessageCollection).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error calling SmsSendPost: %v\n", err)
		return
	}
	fmt.Println(result)
}
```

## Authentication

The API uses HTTP Basic authentication — your ClickSend **username** and **API key** (available from the [ClickSend Dashboard](https://dashboard.clicksend.com/#/account/subaccount)).

## Documentation

Full API reference: https://developers.clicksend.com/docs/rest/v3/

## Support

Need help? Contact [ClickSend Support](https://clicksend.com/contact) or visit the [Help Centre](https://help.clicksend.com/).
