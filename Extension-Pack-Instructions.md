# Windows Extension Pack Download Instructions 🪟
**Delete everything in your `~/.cache/lm-studio/extensions/backends` directory first to ensure new extension packs are installed properly.**
  - Enable **AMD ROCm** for Windows by running the following command in Powershell before starting the app:
  ```
  Invoke-Expression ([System.Text.Encoding]::UTF8.GetString((Invoke-WebRequest -Uri https://files.lmstudio.ai/windows/extension-pack-install-scripts/win-rocm-0.2.25-ext-install.ps1 -  UseBasicParsing).Content))
  ```
  - Enable **OpenCL** for Windows by running the following command in Powershell before starting the app:
  ```
  `Invoke-Expression ([System.Text.Encoding]::UTF8.GetString((Invoke-WebRequest -Uri https://files.lmstudio.ai/win-opencl-ext-install.ps1 -UseBasicParsing).Content))`
  ```
# Linux Extension Pack Download Instructions 🐧
**Delete everything in your `~/.cache/lm-studio/extensions/backends` directory first to ensure new extension packs are installed properly.**
  - Enable **AMD ROCm** for Linux by running the following command in terminal before starting the app:
  ```
  curl -fsSL https://files.lmstudio.ai/linux/0.2.25/beta/extension-pack-install-scripts/lin-rocm-0.2.25-ext-install.sh | sh
  ```
  - Enable **OpenCL** for Linux by running the following command in terminal before starting the app:
  ```
  curl -fsSL https://files.lmstudio.ai/linux/0.2.25/beta/extension-pack-install-scripts/lin-opencl-0.2.25-ext-install.sh | sh
  ```
