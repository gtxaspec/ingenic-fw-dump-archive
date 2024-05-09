# Ingenic Firmware Archive

This repository is dedicated to archiving firmware for Ingenic-based retail devices found in the wild.

## Submission Guidelines

We accept submissions via pull requests that follow the specified directory and file structure outlined below.

### Directory Structure

The directory structure for each submission should be as follows:

```
[BRAND/VENDOR]_[MODEL1]_[MODEL2]_v[HWVER]_[FLASHSIZE]M/
  ├── 0-[BRAND/VENDOR]_[MODEL1]_[MODEL2]_v[HWVER]_[FLASHSIZE]M.bin
  ├── 1-[BRAND/VENDOR]_[MODEL1]_[MODEL2]_v[HWVER]_[FLASHSIZE]M.bin.sha256
  ├── 2-[BRAND/VENDOR]_[MODEL1]_[MODEL2]_v[HWVER]_[FLASHSIZE]M-photo-[desc]-[x].png
  └── 2-[BRAND/VENDOR]_[MODEL1]_[MODEL2]_v[HWVER]_[FLASHSIZE]M-photo-[desc]-fcc-[x].png
```

### File Descriptions

- **`0-[BRAND/VENDOR]_[MODEL1]_[MODEL2]_v[HWVER]_[FLASHSIZE]M.bin`**
  - This is the firmware dump file.

- **`0-[BRAND/VENDOR]_[MODEL1]_[MODEL2]_v[HWVER]_[FLASHSIZE]M-[x].bin`**
  - Some advanced devices may include more than one flash chip onboard. Use `[x]` as an index if multiple dumps are included.

- **`1-[BRAND/VENDOR]_[MODEL1]_[MODEL2]_v[HWVER]_[FLASHSIZE]M.bin.sha256`**
  - This file contains the SHA-256 checksum of the firmware file for integrity verification.

- **`2-[BRAND/VENDOR]_[MODEL1]_[MODEL2]_v[HWVER]_[FLASHSIZE]M-photo-[desc]-[x].png`**
  - These are photos of the logic board. Include as many descriptive photos as possible, using `[desc]` to describe the photo and `[x]` as an index if multiple photos are included.

- **`2-[BRAND/VENDOR]_[MODEL1]_[MODEL2]_v[HWVER]_[FLASHSIZE]M-photo-[desc]-fcc-[x].png`**
  - If you don't have any photos, please include photos from the FCC database for reference. Use `[desc]` to describe the photo and `[x]` as an index if multiple photos are included.

### Example Layout

```
└── WUUK_SAMPLE_DEVICE_v1_02_16M
    ├── 0-WUUK_SAMPLE_DEVICE_v1_02_16M.bin
    ├── 0-WUUK_SAMPLE_DEVICE_v1_02_16M-1.bin
    ├── 0-WUUK_SAMPLE_DEVICE_v1_02_16M-2.bin
    ├── 1-WUUK_SAMPLE_DEVICE_v1_02_16M.bin.sha256
    ├── 2-WUUK_SAMPLE_DEVICE_v1_02_16M-photo-board-1.jpg
    ├── 2-WUUK_SAMPLE_DEVICE_v1_02_16M-photo-board-2.jpg
    ├── 2-WUUK_SAMPLE_DEVICE_v1_02_16M-photo-board-fcc-1.jpg
    └── 2-WUUK_SAMPLE_DEVICE_v1_02_16M-photo-board-fcc-2.jpg
```

## Disclaimer

The firmware and related files in this repository are intended for research purposes only. By contributing to this repository, you agree to use the content responsibly and ethically.

This repository is meant for user-generated firmware dumps and not for retail firmware, as retail firmware typically does not include the bootloader and other critical components. Please ensure that your submissions are generated from your own devices.

**Note**: Some firmware dumps may contain unique serial numbers, encryption keys, or other identifiers. By contributing to this repository, you acknowledge that these identifiers may be exposed and take responsibility for ensuring that you are not violating any terms of service, privacy policies, or other agreements. Additionally, be aware that account credentials may be compromised as a result of exposing these identifiers. No warranty is implied, and contributing is at your own risk.

---

Please ensure your submission adheres to this structure to be accepted into the repository. Thank you for your contributions!
