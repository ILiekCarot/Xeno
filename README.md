> [!WARNING]
> As of August 28 2024, this has been patched. Use this repository to understand what's happening and how it works.

# Xeno
An executor made for the web version of Roblox.

It uses the common method of writing unsigned bytecode into a Roblox core module script to manage execution, also more stable and flexible than most executors that has used this exact method.

## Features
- Fast execution
- Easily detected by Byfron
- Multi-instance compatibility
- Supports executing most scripts including Lua Armor scripts
- No in-game performance change & no high CPU usage

I have only used this project to learn C++ and a bit of C#.

Do not expect the best code and memory management.
You will see really bad code and design on the XenoUI C# WPF project since it was only made as a **prototype**.

This executor has many vulnerabilities because only I have used **Xeno** and did not make a public release.

### Preview
<p>This is the UI of the first release:</p>
<img src="Preview.png" alt="Preview" width="600" style="box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.5), -10px -10px 20px rgba(255, 255, 255, 0.3);" />

## Dependencies
This project uses the following libraries:

- [**httplib**](https://github.com/yhirose/cpp-httplib)
- [**xxhash**](https://github.com/Cyan4973/xxHash)
- [**zstd**](https://github.com/facebook/zstd)

Dependencies are managed with [**vcpkg**](https://github.com/microsoft/vcpkg). Install them with this command:
```sh
vcpkg install xxhash zstd
```

The proper version of **httplib** is already included inside this project

### Credits
Thank you [**Incognito**](https://github.com/Incognito-Roblox/Incognito) for the method.

Thanks to others that has helped me with decompressing, and compressing the bytecode.

Thanks to the [**Init script**](https://github.com/plusgiant5/TaaprWareV2/blob/main/Release/bin/InitScript.lua) of [TaaprWareV2](https://github.com/plusgiant5/TaaprWareV2/) by plusgiant5