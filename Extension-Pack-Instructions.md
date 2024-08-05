# LM Studio - Extension Packs (Beta)

Extension Packs (in public beta) allow you to download LM runtimes that don't come prebundled with LM Studio.

### Available extensions

- [AMD ROCm on Windows](#amd-rocm)
- [AMD ROCm on Linux](#amd-rocm-1)
- [AVX-only CUDA on Linux](#cuda-avx-only)
- [AVX-only CPU on Linux](#cpu-avx-only)

Deprecated:
- [OpenCL on Windows (no longer updated - v0.2.25)](#opencl-0225-does-not-support-gemma-2-or-llama-31)


### One-time step if you've downloaded an extension pack before
Please **first** delete everything in your `%USERPROFILE%\.cache\lm-studio\extensions\backends` (Windows) or `~/.cache/lm-studio/extensions/backends` (Linux) directory to ensure new extension packs are installed properly. 

This is a temporary step.

### Installation on Windows (0.2.31) 🪟

- #### AMD ROCm
Run the following command in Powershell **before** starting the app:
```ps1
Invoke-Expression ([System.Text.Encoding]::UTF8.GetString((Invoke-WebRequest -Uri https://files.lmstudio.ai/windows/extension-pack-install-scripts/win-rocm-0.2.31-ext-install.ps1 -UseBasicParsing).Content))
```
To ensure your new GPU-enabled extension pack is the active LM-Runtime, navigate to `Settings` -> `Advanced Configuration` -> `GPU Settings` -> `GPU Backend Type`, and select it with right-click:

<img src="https://github.com/user-attachments/assets/986fbc1b-abd9-47d4-a0b3-7faf071cfb6f" width="800">

- #### OpenCL (0.2.25, does not support `Gemma 2` or `Llama 3.1`)
Run the following command in Powershell **before** starting the app:
```ps1
Invoke-Expression ([System.Text.Encoding]::UTF8.GetString((Invoke-WebRequest -Uri https://files.lmstudio.ai/win-opencl-ext-install.ps1 -UseBasicParsing).Content))
```

### Installation on Linux (0.2.31) 🐧

- #### AMD ROCm

Run the following command in your terminal **before** starting the app:
```shell
curl -fsSL https://files.lmstudio.ai/linux/0.2.31/beta/extension-pack-install-scripts/lin-rocm-0.2.31-ext-install.sh | sh
```
To ensure your new GPU-enabled extension pack is the active LM-Runtime, navigate to `Settings` -> `Advanced Configuration` -> `GPU Settings` -> `GPU Backend Type`, and select it with right-click:

<img src="https://github.com/user-attachments/assets/986fbc1b-abd9-47d4-a0b3-7faf071cfb6f" width="800">

- #### CUDA AVX-Only

Run the following command in your terminal **before** starting the app:
```shell
curl -fsSL https://files.lmstudio.ai/linux/0.2.31/beta/extension-pack-install-scripts/lin-cuda-avx-0.2.31-ext-install.sh | sh
```

- #### CPU AVX-Only

Run the following command in your terminal **before** starting the app:
```shell
curl -fsSL https://files.lmstudio.ai/linux/0.2.31/beta/extension-pack-install-scripts/lin-cpu-avx-0.2.31-ext-install.sh | sh
```

## Need help?
Join the [LM Studio discord server](https://discord.gg/pwQWNhmQTY) and ask on the `#dev-chat` channel.
