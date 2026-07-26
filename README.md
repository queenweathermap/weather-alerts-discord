# Weather Alerts to Discord

Google アラートRSS（気象防災）をDiscordへ自動配信する仕組みです。
[queenworks/google-alerts-discord](https://github.com/queenworks/google-alerts-discord) から天気防災フィード（`weather-global`）のみを切り出したものです。

## 構成

```text
Googleアラート RSS
↓
GitHub Actions
↓
Python
↓
Discord Webhook
```

## 入っているファイル

```text
google_alerts_to_discord.py
feeds.json
requirements.txt
.github/workflows/google_alerts_discord.yml
state/.gitkeep
```

## 必要なSecrets

- `RSS_WEATHER_GLOBAL`
- `DISCORD_WEATHER_BOSAI_WEBHOOK`

（元の`queenworks/google-alerts-discord`のリポジトリSecretsから同じ値をコピーしてください）
