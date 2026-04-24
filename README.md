# CEngine

A fast bitboard-based chess engine with GPU-accelerated legal move generation (HIP).

## Quick Start (Windows - Recommended)

### Pre-built Portable Version (no admin rights needed)
1. Go to the [Releases](https://github.com/yourusername/CEngine/releases) page
2. Download the latest `CEngine-1.0.0-win64.zip`
3. Unzip it anywhere (Desktop, Documents, USB stick — anywhere)
4. Run `CEngine.exe`

**Requirements:**
- AMD GPU with a recent Adrenalin driver (RX 7600 and most modern AMD cards work great)
- For NVIDIA GPUs: see "Building from source" below

### Building from Source (for developers)

1. Install the **AMD HIP SDK** (free developer tools):
   - Download from: https://www.amd.com/en/developer/resources/rocm-hub/hip-sdk.html
   - Choose the latest Windows 11 version (or Windows 10/11 compatible)
   - Run the installer (no admin required for building if you use user paths)

2. Open the project in CLion (or any CMake-compatible IDE)
3. Configure and build in **Release** mode
4. Done — the executable will be in the build folder

NVIDIA users: Install the NVIDIA CUDA Toolkit as well, then build with `-DHIP_PLATFORM=nvidia`.

## Features
- GPU-accelerated legal move generation
- Supports castling, en passant, 50-move rule, 3-fold repetition
- Highly portable HIP code (AMD native + NVIDIA compatible)

Enjoy!
