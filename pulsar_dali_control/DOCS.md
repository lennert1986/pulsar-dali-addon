# Pulsar DALI Control documentation

## Default connections

| Function | Device |
|---|---|
| DALI 1 | `/dev/ttyAMA3` |
| DALI 2 | `/dev/ttyAMA4` |
| DALI 3 | `/dev/ttyAMA5` |

UART: 115200 baud, 8N1.

## First start

1. Start the App.
2. Open the Pulsar DALI web UI.
3. Verify all three DALI buses are online.
4. Run **Scan all buses**.

## Remote access

Remote API is disabled by default. When enabled it uses HTTPS, bearer-token authentication and SHA-256 certificate fingerprint pinning on TCP port 8443.

Treat the remote token as a password because it grants full API access.
