# ngrok-cheat-sheet
ngrok-cheat-sheet


# Install

## Ubuntu
```shell
curl -sSL https://ngrok-agent.s3.amazonaws.com/ngrok.asc \
  | sudo tee /etc/apt/trusted.gpg.d/ngrok.asc >/dev/null \
  && echo "deb https://ngrok-agent.s3.amazonaws.com buster main" \
  | sudo tee /etc/apt/sources.list.d/ngrok.list \
  && sudo apt update \
  && sudo apt install ngrok
```

Then:
```shell
ngrok config add-authtoken xxxxxxxxxxx
```




<br><br>
<br><br>
___
<br><br>
<br><br>




# Serve

<br><br>

## Serve local port
```shell
ngrok http 3000
```














<br><br>
<br><br>
___
<br><br>
<br><br>



# Auth

<details><summary>Click to expand..</summary>

<br><br>

## Basic Auth
- https://ngrok.com/docs/http/basic-auth/
```shell
ngrok http 11434 \
  --basic-auth "test:tesxxxxxxxxxxxxxfe" \
  --host-header="localhost:11434"
```
```shell
curl https://xxxxxxxxx46.ngrok-free.app/v1/chat/completions \
    --user "testtesxxxxxxxxxxxxxfe" \
    -H "Content-Type: application/json" \
    -d '{
        "model": "llama2",
        "messages": [
            {
                "role": "system",
                "content": "You are a helpful assistant."
            },
            {
                "role": "user",
                "content": "Hello!"
            }
        ]
    }'
```


</details>


