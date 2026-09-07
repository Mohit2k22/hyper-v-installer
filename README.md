# Hyper-V Installer for Windows

A simple Windows batch script for installing Hyper-V packages and enabling the Microsoft Hyper-V Windows feature using DISM.

## Requirements

- Windows with Hyper-V packages available under `%SystemRoot%\servicing\Packages`
- Administrator privileges
- A supported Windows edition with Hyper-V capability

## Usage

1. Download or clone this repository.
2. Run `hyper-v.bat` as **Administrator**.
3. Allow DISM to complete the package installation and feature enablement.
4. Restart Windows if required.

## What the script does

The script:

1. Changes to its own directory.
2. Finds Hyper-V `.mum` packages in the Windows servicing package directory.
3. Installs the discovered packages with DISM.
4. Enables the `Microsoft-Hyper-V` feature and its dependencies.
5. Pauses so the output can be reviewed.

## Important

This script modifies Windows components. Run it with Administrator privileges and use it only when you understand the changes it makes to the system.

## License

This project is released under the MIT License. See `LICENSE` for details.
