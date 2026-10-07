# ionCube Decoder v15

https://github.com/user-attachments/assets/467276e1-159d-4187-84b5-54300fe938b0

An independent decoder and PHP source reconstructor for supported ionCube
Encoder formats. It provides a simple web interface for uploading encoded PHP
files, reviewing reconstructed code, and downloading individual PHP files or a
ZIP archive.

> This is a public product showcase. Decoder source code and commercial
> binaries are not distributed in this repository.

## Features

- Simple browser-based decoding workflow
- Multiple-file and ZIP processing
- Reconstructed PHP preview and download
- Searchable decode history with clear failure diagnostics
- REST API for automated file decoding
- Native Go application with Docker deployment support
- Local and self-hosted operation
- Checksum and profile validation before reconstruction

## Compatibility

| ionCube Encoder | Verified PHP targets |
| --- | --- |
| 10.2.0 | 7.2 |
| 10.2.2 | 7.1, 7.2 |
| 11.0.2 | 7.1, 7.2 |
| 12.0.2 | 8.1 |
| 13.0.1 | 7.4, 8.1, 8.2 |
| 13.0.2 | 7.1, 7.2, 7.4, 8.1, 8.2 |
| 13.0.3 | 7.4, 8.1, 8.2 |
| 14.0.1 | 7.4, 8.1, 8.2 |
| 14.0.2 | 7.1, 7.2, 7.4, 8.1, 8.2, 8.3 |
| 15.0.1 | 7.1, 7.2, 7.4, 8.1, 8.2, 8.3, 8.4 |

Compatibility depends on the encoded format, protection options, and PHP
constructs used by each file. Reconstructed output preserves program behavior
for supported profiles, but exact formatting and source information removed
during encoding cannot always be recovered.

## How it works

1. The decoder identifies the Encoder and PHP target profile.
2. It validates and extracts the protected container and bytecode records.
3. It reconstructs supported instructions, declarations, expressions, and
   control flow as readable PHP.
4. The completed PHP is made available for preview or download; unsupported
   input returns a specific diagnostic instead of incomplete placeholder code.

## Demo video

The repository includes the original H.264 walkthrough at
[`docs/media/decoding-demo.mp4`](docs/media/decoding-demo.mp4).

## Purchase and contact

The decoder is available as commercial software. For pricing, licensing, and
deployment options, contact **[@amirmalek0](https://t.me/amirmalek0)** on
Telegram.

---

ionCube is a trademark of ionCube Ltd. This independent project is not
affiliated with or endorsed by ionCube Ltd.
