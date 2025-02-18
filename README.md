# EFINextBoot
Reimplementation of [chengxuncc/booToLinux](https://github.com/chengxuncc/booToLinux) with zero-dependency in mind  
Using `bcdedit` internally to select the next time boot of UEFI: ```bcdedit /set {fwbootmgr} bootsequence {GUID}```

## What's new?
- useable in non-english windows
- add possible parameter /L to display EFI-content
  
## Download
Download prebuilt binary: [Releases](https://github.com/Hubhubhurra/efinextboot/releases)

## Build 
```dos
go build
```

## Build with Administrator privileges
```dos
go build github.com/akavel/rsrc
rsrc.exe -manifest efinextboot.exe.manifest -o efinextboot.exe.syso
go build
```
Double click to run.

## License
EFINextBoot is licensed under the MIT license.
