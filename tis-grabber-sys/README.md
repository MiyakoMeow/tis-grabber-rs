# A Rust bindings for **IC Imaging Control 4 SDK** from [The Imaging Source](https://www.theimagingsource.com/)

For Windows platform, bindings from C headers.

## Build & Run Requirement

Download, install with all default presets.

Then ensure that the `bin` directory of the SDK and Driver is in the `PATH` variable.

### 1. SDK

- IC Imaging Control Legacy SDK: [](<https://www.theimagingsource.com/zh-hans-cn/support/download/icimagingcontrol4win-1.1.0.2833/>)

### 2. Driver

- For GigE Devices: [](<https://www.theimagingsource.com/zh-hans-cn/support/download/ic4gentlprodgevwintis-1.3.0.821/>)
- For USB3 Devices: [](<https://www.theimagingsource.com/zh-hans-cn/support/download/ic4gentlprodu3vwintis-1.3.0.480/>)

For more infomation, see [](<https://www.theimagingsource.com/zh-hans-cn/support/download/>)

## Notice

1. Call `tis_grabber_sys::ic4_init_library` before calling any other function.
2. If possible, **DO NOT** use value in this crate generated from `Default::default`,
as the value is from non-zerolized memory spaces.
