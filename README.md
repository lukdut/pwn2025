# pwn2025

<p align="center">
  <strong>English</strong> · <a href="README.ru.md">Русский</a>
</p>

A large Wi-Fi password dictionary compiled from **rockyou2024** and other
sources. All entries are unique and sorted by length, then alphabetically.

> [!IMPORTANT]
> Use this dictionary only to audit systems and networks you own or are
> explicitly authorized to test.

## Downloads

| Edition | Passwords | Length | Download size | Unpacked size |
| --- | ---: | ---: | ---: | ---: |
| [`pwn2025.1`](pwn2025.1.torrent) — split `.xz` files | 22,041,027,703 | 8–32 characters | ≈ 40 GiB | ≈ 281 GiB |
| [`pwn2025.rar`](pwn2025.rar.torrent) — single RAR archive | 18,437,789,173 | up to 63 characters | ≈ 56 GiB | ≈ 269 GiB |

### `pwn2025.1`

The split edition lets you select only the password-length ranges you need in
your BitTorrent client. Its `.xz` files can be passed directly to Hashcat, so
they do not need to be unpacked first. You can provide more than one file at a
time.

```console
hashcat [options] <hash-file> pwn2025.1_8_9.txt.xz
hashcat [options] <hash-file> pwn2025.1_8_9.txt.xz pwn2025.1_10a.txt.xz
hashcat [options] <hash-file> pwn2025.1/
```

The last command uses every dictionary file in the `pwn2025.1` directory. The
exact command and options depend on the hash type and attack mode.

#### File structure

| File | Password length | Lines | Bytes unpacked |
| --- | ---: | ---: | ---: |
| `pwn2025.1_8_9.txt` | 8–9 | 4,174,820,727 | 39,782,726,938 |
| `pwn2025.1_10a.txt` | 10 (first half) | 3,112,253,707 | 34,234,790,777 |
| `pwn2025.1_10b.txt` | 10 (second half) | 3,112,253,707 | 34,234,790,777 |
| `pwn2025.1_11.txt` | 11 | 2,185,100,119 | 26,221,201,428 |
| `pwn2025.1_12.txt` | 12 | 2,030,722,773 | 26,399,396,049 |
| `pwn2025.1_13_14.txt` | 13–14 | 2,464,406,845 | 35,629,670,412 |
| `pwn2025.1_15_16.txt` | 15–16 | 1,895,721,654 | 31,365,037,873 |
| `pwn2025.1_17_23.txt` | 17–23 | 1,813,428,393 | 36,887,728,511 |
| `pwn2025.1_24_29.txt` | 24–29 | 703,421,855 | 18,725,007,503 |
| `pwn2025.1_30_32a.txt` | 30–32 (first half) | 274,448,961 | 8,988,795,591 |
| `pwn2025.1_30_32b.txt` | 30–32 (second half) | 274,448,962 | 9,056,815,746 |
| **Total** | **8–32** | **22,041,027,703** | **301,525,961,605** |
