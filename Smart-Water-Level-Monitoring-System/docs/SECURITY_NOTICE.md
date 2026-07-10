# Security Notice

## Credentials Are Embedded in the Supplied Sketch

The original `esp32_blynk.ino` contains:

- A Blynk authentication token
- A Wi-Fi SSID
- A Wi-Fi password

The source file in this repository was copied exactly as supplied, in accordance with the requirement not to alter the code.

## Before Publishing This Repository

1. Revoke or regenerate the exposed Blynk device token.
2. Change the Wi-Fi password if it is still active.
3. Replace the credential values before making the repository public.
4. Prefer moving credentials into a private `secrets.h` file in a future revision.
5. Add `secrets.h` to `.gitignore`.
6. Do not commit screenshots containing tokens, QR codes, passwords, or device identifiers.

A public GitHub commit remains accessible through repository history even after a later edit. Remove credentials before the first public commit, or rewrite the repository history if they have already been committed.
