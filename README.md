# NTLMX

[![PowerShell Gallery](https://img.shields.io/powershellgallery/v/NTLMX.svg)](https://www.powershellgallery.com/packages/NTLMX) ![](https://img.shields.io/badge/supported%20windows%20versions-7%2F8%2F10-green.svg)

Post-exploitation NTLM password hash extractor.

## Description

Extract local NTLM user password hashes from the registry handling latest AES-128-CBC with IV obfuscation techniques introduced with Windows 10 1607 as well as the traditional MD5/RC4 approach used in Windows 7/8/8.1.

**Note:** Requires to be run as `SYSTEM`.

See [ImpersonateSystem](https://github.com/off-world/ImpersonateSystem) to accomplish that from within an elevated context.

## Supported Target Systems
So far the script has been tested to work on:
-  Windows 10 1809 with PowerShell 5.1
-  Windows 8.1 with PowerShell 4.0
-  Windows 7 with PowerShell 2.0

## Installation

Install from [PowerShell Gallery](https://www.powershellgallery.com/packages/NTLMX)

```Powershell
Install-Module -Name NTLMX
```
or
```Shell
git clone https://github.com/tobiohlala/NTLMX
```

## Usage

```Powershell
Import-Module NTLMX

Get-NTLMLocalPasswordHashes
```

## Examples

```Powershell
Get-Help Get-NTLMLocalPasswordHashes -Examples
```
