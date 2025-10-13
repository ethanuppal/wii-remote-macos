## Preliminaries

- You will probably need to buy the Dolphinbar. The official manufacturer is Mayflash. Here is an Amazon link that I found: https://www.amazon.com/Mayflash-W010-Wireless-Sensor-DolphinBar/dp/B00HZWEB74/
- Please note that all users referenced here are either available on public sites or public forums.
- Starting from macOS 12.0, Apple dropped support for legacy bluetooth.[^1] Users running earlier versions seem to have had no issues connecting Wii remotes[^4].

## Prior Solutions

- Dolphin has an unmaintained repository for an app called [WiimotePair](https://github.com/dolphin-emu/WiimotePair). Some users reported success with using this app[^5] — even being able to pair the balance board[^6] — but I was unable to get it to work.
- There is an app called [WiiController](https://github.com/WiiController/WiiController) that a user reported as being essential to connecting with WiimorePair.[^6]
  - They first paired their remote with [this download of WiiController](https://github.com/WiiController/WiiController/files/8007293/WiiController.dmg.zip) (which has a branch for experimenting with macOS 12+ support).
  - They signed the app and opened it, which was necessary to get macOS to recognize the remote as a magic trackpad. (I was unable to replicate this; the signed app did not open.)

## Papercuts

- Disable the Wii remote speakers. According to `@Melumi`[^2], they "make crackling sounds which is distracting". Furthermore, according to `@Hibyehello`[^3], getting them to work at all requires "bluetooth passthrough", unavailable on later versions of macOS.

## Support

A "No" in a column means that the user has been unsuccessful at using that method.
A "Yes" in any column means that the user has been successful at using that method.
In particular, if there 

Model | OS | Dolphin | Remote | WiimotePair |  Dolphinbar | Other adapter | User | Date updated
--- | --- | --- | --- | --- | --- | --- | --- | ---
M3 Air | 14.7 | 2509 | | No |  | | Me | 2025 
M3 Pro | 15   |      | |    | Yes | | `@Melumi`[^2] | 2025 
M3 ? | 14.3.1 | 5.0-21116  | | Yes[^4] | | | `sejmann74` | 2024 
M4 Mini | 26.0.1 | 2509-178 | RVL-036 2025 | | | Yes, TP-Link UB400 | `@Amy`[^7]

## Sources

[^1]: https://github.com/dortania/OpenCore-Legacy-Patcher/issues/364
[^2]: Discord: 640714673045504020
[^3]: Discord: 683825611566874641
[^4]: https://bugs.dolphin-emu.org/issues/12662
[^5]: https://github.com/dolphin-emu/WiimotePair/issues/14
[^6]: https://github.com/dolphin-emu/WiimotePair/issues/1
[^7]: Discord: 1203712057640357898
