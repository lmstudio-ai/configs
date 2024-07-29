## LM Studio - Extension Packs (Beta)

### One-time step if you have downloaded an extension pack before
Please **first** delete everything in your `%USERPROFILE%\.cache\lm-studio\extensions\backends` (Windows) or `~/.cache/lm-studio/extensions/backends` (Linux) directory to ensure new extension packs are installed properly. 

This is a temporary step.

## Installation on Windows (0.2.29) 🪟

- #### AMD ROCm
Run the following command in Powershell **before** starting the app:
```ps1
Invoke-Expression ([System.Text.Encoding]::UTF8.GetString((Invoke-WebRequest -Uri https://files.lmstudio.ai/windows/extension-pack-install-scripts/win-rocm-0.2.29-ext-install.ps1 -UseBasicParsing).Content))
```
To ensure you're new GPU-enabled extension pack is the active LM-Runtime, navigate to `Settings` -> `Advanced Configuration` -> `GPU Settings` -> `GPU Backend Type`, and select it with right-click:

<img src="https://github.com/user-attachments/assets/986fbc1b-abd9-47d4-a0b3-7faf071cfb6f" width="800">


## Installation on Linux (0.2.29) 🐧

- #### AMD ROCm

Run the following command in your terminal **before** starting the app:
```shell
curl -fsSL https://files.lmstudio.ai/linux/0.2.29/beta/extension-pack-install-scripts/lin-rocm-0.2.29-ext-install.sh | sh
```
To ensure you're new GPU-enabled extension pack is the active LM-Runtime, navigate to `Settings` -> `Advanced Configuration` -> `GPU Settings` -> `GPU Backend Type`, and select it with right-click:

<img src="https://github.com/user-attachments/assets/986fbc1b-abd9-47d4-a0b3-7faf071cfb6f" width="800">

- #### CPU AVX-Only

Run the following command in your terminal **before** starting the app:
```shell
curl -fsSL https://files.lmstudio.ai/linux/0.2.29/beta/extension-pack-install-scripts/lin-cpu-avx-0.2.29-ext-install.sh | sh
```

## Need help?
Join the [LM Studio discord server](https://discord.gg/pwQWNhmQTY) and ask on the `#dev-chat` channel.
