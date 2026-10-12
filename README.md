# 💸 FeePilot — Trading Fee Calculator (MIT)

Interactive crypto & FX fee calculator. UI in EN/TR/AR. Static single file.

## Calculators

- **📊 Spot:** qty × price with maker/taker fee + token & referral discounts
  (multiplicative). Buy total / sell net with full breakdown.
- **⚡ Futures:** open + close fees on notional, margin from leverage,
  optional funding per period.
- **🔁 Transfer/Swap:** flat network (gas) fee + platform % + slippage
  tolerance → net received + effective cost % + risk flags.
- **⚖️ Compare:** same notional across Binance/KuCoin/Bybit/OKX/MEXC/Bitget,
  ranked by total cost. Default fees are **indicative VIP0** — every field
  is user-editable; verify tiers on exchanges.
- **🎁 Referrals:** `CONFIG.refs = { binance: 'https://...your-code...' }`
  per exchange; ★ badge when custom. Empty = official homepage.
  "Trade with lower fees" buttons on every row.

## Money & contact

- `CONFIG.ads` (AdSense/Carbon) footer slot.
- Donate box: BTC + USDT-TRC20 live.
- 📧 baranavisat@gmail.com · 📞 +90 531 326 37 22 · WhatsApp

## Run

```bash
cd feepilot
python3 -m http.server 8080
```

## License

MIT. Not financial advice.

## Telegram (@BaranScanBot)

- Footer'da herkese açık "Telegram" butonu (`t.me/BaranScanBot`) — ziyaretçi
  doğrudan bota yazar, ek ayar gerekmez.
- Sipariş/satış bildirimleri (`tgSend`) yalnızca `CONFIG`... `TG.chat`
  doluysa sahibine gider. Chat ID'yi @userinfobot'tan alıp `TG.chat`e yazın.
- ⚠️ **GÜVENLİK:** Bot tokeni herkese açık istemci kodundadır; kaynağı
  gören herkes bot adına mesaj gönderebilir. Kötüye kullanımda BotFather'dan
  tokeni yenileyin ve asla bu botla hassas işlem yapmayın. Gerçek çözüm:
  backend proxy.
