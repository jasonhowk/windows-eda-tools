# windows-eda-tools

A Scoop bucket providing Electronic Design Automation (EDA) tools for Windows: Icarus Verilog, Digital, and GTKWave 4.

The packages are distributed as pre-built Windows artifacts so installation does not require a compiler or local build environment.

## Install

Install [Scoop](https://scoop.sh/) from a regular, non-administrator PowerShell session:

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
irm get.scoop.sh | iex
```

Add this bucket:

```powershell
scoop bucket add java
scoop bucket add eda-tools https://github.com/jasonhowk/windows-eda-tools
```

## Tools

### Icarus Verilog

A Verilog HDL compiler and simulator.

```powershell
scoop install eda-tools/icarus-verilog
```

### Digital

A visual digital logic designer and circuit simulator.

```powershell
scoop install eda-tools/digital
```

### GTKWave 4

A waveform viewer for inspecting VCD and FST output files from Verilog/VHDL simulations.

```powershell
scoop install eda-tools/gtkwave4
```

## Install all tools

```powershell
scoop install eda-tools/icarus-verilog eda-tools/digital eda-tools/gtkwave4
```

## Architecture

Native Windows x64 (`x86_64`) packages are provided. Windows 11 ARM64 systems may run the x64 packages through Windows emulation. Native ARM64 packages and 32-bit Windows packages are not currently provided.

## Releases

Windows artifacts are published through [GitHub Releases](https://github.com/jasonhowk/windows-eda-tools/releases). Scoop verifies downloaded artifacts using SHA-256 hashes.

## Related project

The macOS packages are available from the [homebrew-eda-tools](https://github.com/jasonhowk/homebrew-eda-tools) Homebrew tap.
