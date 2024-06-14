## LM Studio - Extension Packs (Beta)

### One-time step for LM Studio 0.2.24 -> 0.2.25 upgrade
If you've downloaded an extension pack before, please **first** delete everything in your `~/.cache/lm-studio/extensions/backends` directory to ensure new extension packs are installed properly. 

This is only required for this release.

## Installation on Windows 🪟

- #### AMD ROCm
Run the following command in Powershell **before** starting the app:
```ps1
Invoke-Expression ([System.Text.Encoding]::UTF8.GetString((Invoke-WebRequest -Uri https://files.lmstudio.ai/windows/extension-pack-install-scripts/win-rocm-0.2.25-ext-install.ps1 -  UseBasicParsing).Content))
```

- #### OpenCL
Run the following command in Powershell **before** starting the app:
```ps1
Invoke-Expression ([System.Text.Encoding]::UTF8.GetString((Invoke-WebRequest -Uri https://files.lmstudio.ai/win-opencl-ext-install.ps1 -UseBasicParsing).Content))
```

## Installation on Linux 🐧 

- #### AMD ROCm

Run the following command in your terminal **before** starting the app:
```shell
curl -fsSL https://files.lmstudio.ai/linux/0.2.25/beta/extension-pack-install-scripts/lin-rocm-0.2.25-ext-install.sh | sh
```
- #### OpenCL
Run the following command in your terminal **before** starting the app:

```shell
curl -fsSL https://files.lmstudio.ai/linux/0.2.25/beta/extension-pack-install-scripts/lin-opencl-0.2.25-ext-install.sh | sh
```

## Need help?
Join the [LM Studio discord server](https://discord.gg/pwQWNhmQTY) and ask on the `#dev-chat` channel.
