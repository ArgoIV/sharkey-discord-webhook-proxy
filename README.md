# Sharkey Discord Webhook Proxy

The proxy to send discord Webhook from Sharkey.

This proxy supports sending discord message from Sharkey note webhook.

## How to use (server)

1. build with `cargo build --release`
2. `./target/release/misskey-discord-webhook-proxy <listen addr & port>`

## How to use (proxy)

Discord will give you a webhook URL, such as
`https://discord.com/api/webhooks/1143087113424879627/adffadjkdfllandjkfkjadjklf`.
The webhook_id is `1143087113424879627` and the webhook_secret is `adffadjkdfllandjkfkjadjklf` in this example

Configure your Sharkey webhook with `http://<prox-server>/discord/<webhook_id>/Sharkey` as your URL, and `<webhook_token>` as your secret.
