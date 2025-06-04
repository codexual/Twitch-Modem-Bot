# Interface Status and Speed Test Bot

This bot provides real-time monitoring of network interfaces and speed tests for various network providers. It includes commands to check interface statuses, run speed tests, and analyze connection performance.

On Line 272, and 278. Please put in your IP Address/DDNS/Domain name, that block of code (snippet) will ping your server and shows if it's online or not. No Actual IP Address, DDNS, and or Domain Name will(not) show in your Twitch Chat.

## Features
- **Interface Monitoring:** View real-time TX and RX speeds for multiple network interfaces.
- **Speed Testing:** Run speed tests for supported providers with minimal output.
- **Connection Stability Checks:** Ping fiber and coax networks to verify connection stability.
- **Historical Data:** Retrieve the last five speed test results for a given provider.

## Interface Status Commands
These commands display real-time TX and RX speeds for a specific interface:

- `!modem` - Displays the overall network status for all interfaces, including provider names, TX/RX speeds, and connection status indicators (✅ OK, ⚠️ SLOW, ❌ DOWN).
- `!verizon` - Displays TX/RX speeds for Verizon (`wlan0`).
- `!tmobile` - Displays TX/RX speeds for T-Mobile (`wlan1`).
- `!att` - Displays TX/RX speeds for AT&T (`wlan2`).
- `!dish` - Displays TX/RX speeds for Dish (`wlan3`).
- `!starlink` - Displays TX/RX speeds for Starlink (`wlan4`).
- `!speedify` - Displays TX/RX speeds for Speedify (`connectify0`).

## Speed Test Commands
These commands run a full speed test for the specified interface and return only latency, download, and upload speeds (moderators and streamer only):

- `!speedtestverizon` - Runs a speed test on Verizon (`wlan0`).
- `!speedtesttmobile` - Runs a speed test on T-Mobile (`wlan1`).
- `!speedtestatt` - Runs a speed test on AT&T (`wlan2`).
- `!speedtestdish` - Runs a speed test on Dish (`wlan3`).
- `!speedteststarlink` - Runs a speed test on Starlink (`wlan4`).
- `!speedtestspeedify` - Runs a speed test on Speedify (`connectify0`).

### Shortened Aliases:
- `!speedverizon` → `!speedtestverizon`
- `!speedtmobile` → `!speedtesttmobile`
- `!speedatt` → `!speedtestatt`
- `!speeddish` → `!speedtestdish`
- `!speedstar` → `!speedteststarlink`
- `!speedsify` → `!speedtestspeedify`

## Other Utility Commands
- `!pingfiber` - Pings `DDNS/DOMAIN` (Fiber) and reports stability.
- `!pingcoax` - Pings `DDNS/DOMAIN` (Coax) and reports stability.
- `!topspeed` - Compares TX/RX speeds across all interfaces and identifies the fastest network.
- `!speedhistory [provider]` - Displays the last five speed test results for a specified provider (e.g., `!speedhistory att`).
- `!usage [interface]` - (Placeholder) Intended to display total data usage for a specific interface (not yet implemented).

## Important Note on Speedify
Speedify is a **paid** subscription service that combines multiple internet connections for improved reliability and performance. Ensure you have an active subscription to use the `!speedify` and `!speedtestspeedify` commands.

## Contribution
Feel free to contribute by submitting issues or pull requests to enhance functionality!

## License
MIT License
