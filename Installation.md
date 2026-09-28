# Python Installation

Follow these steps to install Python on Windows 10 or Windows 11.

## Installation Steps

### 1. Download the Installer

1. Open [python.org/downloads/windows](https://www.python.org/downloads/windows/) in a browser.
2. Select the current stable Python release for Windows.
3. Download the installer that matches your computer. The 64-bit installer is appropriate for most modern PCs.
4. When the download finishes, open the installer from your browser's downloads list or the Downloads folder.

### 2. Install Python

1. In the installer window, select **Add python.exe to PATH** if that option is shown. This makes the `python` command available from a terminal.
2. Select **Install Now** for a typical personal installation. If Windows requests permission, approve it only if you are authorized to install software on this computer.
3. Wait for the installation to complete. Select **Close** when the installer reports success.

If you need to choose a custom location or installation features, use **Customize installation**. Keep the default options unless you have a specific requirement.

## Verification Steps

1. Open a new PowerShell window or Command Prompt. A new window ensures it reads the updated environment settings.
2. Run:

   ```powershell
   python --version
   ```

   The command should print the installed Python version, for example `Python 3.x.x`.
3. Check that the package installer is available:

   ```powershell
   python -m pip --version
   ```

4. If the `python` command is unavailable, try the Windows Python launcher:

   ```powershell
   py --version
   py -m pip --version
   ```

A version number from either `python --version` or `py --version` confirms that Python is installed. Use `python -m pip` (or `py -m pip`) to run pip for that Python installation.

### Run a Small Test

At the terminal prompt, enter:

```powershell
python -c "print('Python is ready')"
```

If you used the launcher instead, run:

```powershell
py -c "print('Python is ready')"
```

The output should be `Python is ready`.

### Installation Checklist

- The installer was downloaded from the official Python website.
- The installer completed without reporting an error.
- A new terminal displays a Python version with `python --version` or `py --version`.
- The pip version command succeeds.
- The short test program prints its expected message.

For common issues, see [Troubleshooting](#troubleshooting) below or the [FAQ](FAQ.md).

## Troubleshooting

### `python` is not recognized

Open a new terminal and try `py --version`. If that works, Python is installed and you can use `py` in place of `python`. Otherwise, rerun the official installer and select **Add python.exe to PATH**, or use the launcher's **Install Now** route from the installer. Avoid manually editing `PATH` unless you know the exact installation directory.

### The Microsoft Store opens when I type `python`

Try `py --version`. Windows may be resolving `python` to an app execution alias. You can turn off the Python aliases in **Settings > Apps > Advanced app settings > App execution aliases**, then open a new terminal and test again. Settings labels can vary by Windows version.

### `pip` is not recognized

Run pip through the interpreter instead of calling `pip` directly:

```powershell
python -m pip --version
```

If `python` is unavailable but `py` works, use `py -m pip --version`.

### A different Python version appears

Use `py --list` to see Python versions registered with the launcher. When more than one version is installed, specify one explicitly, for example `py -3.12 --version`, replacing `3.12` with the version you intend to use.

### Installation fails or asks for administrator access

Confirm that the installer came from python.org and that Windows has enough free disk space. On a school- or work-managed device, contact the administrator rather than trying to bypass installation controls.

## Conclusion

Python is ready to use once the installer completes and the version and test commands succeed. Keep track of the Python version required by each project, and use the official Python documentation when you need platform-specific details or advanced configuration.
