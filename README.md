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

	message := clicksend.NewSendSmsRequestMessagesInner("Hello from ClickSend!")
	message.SetTo("+61411111111")
	message.SetSource("sdk")

	sendSmsRequest := clicksend.NewSendSmsRequest()
	sendSmsRequest.SetMessages([]clicksend.SendSmsRequestMessagesInner{*message})

	result, _, err := client.SmsAPI.SendSms(auth).SendSmsRequest(*sendSmsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error calling SendSms: %v\n", err)
		return
	}
	fmt.Println(result)
}
```

## More Examples

### View account details

```go
result, _, err := client.ManagementAPI.ViewAccountDetails(auth).Execute()
if err != nil {
	fmt.Fprintf(os.Stderr, "Error calling ViewAccountDetails: %v\n", err)
	return
}
fmt.Println(result)
```

### Send an MMS

```go
mmsMessage := clicksend.NewSendMmsRequestMessagesInner()
mmsMessage.SetTo("+61411111111")
mmsMessage.SetFrom("sdk")
mmsMessage.SetSubject("Hello")
mmsMessage.SetBody("Hello from ClickSend!")
mmsMessage.SetSource("sdk")

sendMmsRequest := clicksend.NewSendMmsRequest()
sendMmsRequest.SetMediaFile("https://clicksend.com/logo.png")
sendMmsRequest.SetMessages([]clicksend.SendMmsRequestMessagesInner{*mmsMessage})

result, _, err := client.MmsAPI.SendMms(auth).SendMmsRequest(*sendMmsRequest).Execute()
if err != nil {
	fmt.Fprintf(os.Stderr, "Error calling SendMms: %v\n", err)
	return
}
fmt.Println(result)
```

## Authentication

The API uses HTTP Basic authentication — your ClickSend **username** and **API key** (available from the [ClickSend Dashboard](https://dashboard.clicksend.com/#/account/subaccount)).

## Documentation

Full API reference: https://developers.clicksend.com/docs/rest/v3/

## Support

Need help? Contact [ClickSend Support](https://clicksend.com/contact) or visit the [Help Centre](https://help.clicksend.com/).