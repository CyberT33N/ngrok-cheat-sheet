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
