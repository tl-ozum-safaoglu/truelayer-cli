# truelayer-cli

## Install

```
brew tap tl-ozum-safaoglu/truelayer
brew install truelayer
```

## Use

### Generate webhooks

*Generate executed and settled webhooks*

```
truelayer generate-webhook 
    --private-key {path_to_private_key_pem} 
    --client-id {client_id} 
    --client-secret {client_secret}
    --kid {private_id_key_from_console}
      executed-settled
```

*Generate failed webhook*

```
truelayer generate-webhook 
    --private-key {path_to_private_key_pem} 
    --client-id {client_id} 
    --client-secret {client_secret}
    --kid {private_id_key_from_console}
      failed
```

### Create a tunnel to a local app

Creates an HTTP tunnel to `localhost:8080`

```
 create-tunnel --route-to localhost:8080
```
