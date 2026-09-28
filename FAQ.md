# Frequently Asked Questions

## Is Python free?

Yes. Python is open-source software and can be downloaded from [python.org](https://www.python.org/).

## Which version should I install?

For a new installation, choose the current stable release offered on the official Python downloads page, unless a course, employer, or project specifically requires another version.

## Do I need administrator rights?

Not always. The installer may offer an installation for the current user. A managed computer or an all-users installation may require administrator approval. Follow your organization's software installation policy.

## What does “Add python.exe to PATH” do?

It allows Windows to find Python when you type `python` in a terminal. If you leave it unchecked, the `py` launcher may still work, or you may need to select Python's install location when running it.

## What is the `py` command?

The Python launcher for Windows can find registered Python installations and select a version. For example, `py --version` displays a version, and `py -m pip --version` checks pip for the launched interpreter.

## What is pip?

`pip` is Python's package installer. It downloads and installs third-party packages. Calling it as `python -m pip` helps ensure it belongs to the Python interpreter you are using.

## How can I tell whether Python installed correctly?

Open a new PowerShell or Command Prompt window and run `python --version`. If that command is not found, try `py --version`. Then test a short command such as `py -c "print('Python is ready')"`.

## Can I install more than one Python version?

Yes. Multiple versions can be installed. Use `py --list` to see versions recognized by the launcher, and `py -3.x` to select a specific version where available.

## Do I need to install an editor?

No. Python can run from a terminal. A code editor or IDE is optional, though it can make writing and managing programs more convenient.

## Where should I get help if installation still fails?

Review [Installation.md](Installation.md#troubleshooting), then consult the official [Python documentation](https://docs.python.org/3/using/windows.html) or ask the administrator of a managed device.
