# SeedVR2 — AMD port (Radeon 8060S)

One-click Windows installer for SeedVR2, ported from NVIDIA-only to AMD. Free.

## What it does

SeedVR2 is a video upscaler — it takes a low-resolution video and produces a larger, cleaner one, in a single step.

## Tested on

- AMD Ryzen AI Max+ 395 with Radeon 8060S (gfx1151)
- BOSGAME M5

Reported test results from our developer team's testing on that machine: an installed GPU run upscaled 48 frames from 320×240 to 640×480 in about 174 seconds, peaking at about 8.4 GiB of graphics memory; silent install and uninstall passed.

## Before you install

**You need the AI Video Suite installed first.** This port uses the Suite's ROCm Python and SeedVR2 weights read-only. On install it downloads the pinned ComfyUI files it needs; if the weights are not already present, it downloads the official SeedVR2 files.

**Hardware check — please read first.** The installer checks your hardware before it installs. This build is made for a machine with an AMD Radeon 8060S (gfx1151) and the Suite's PyTorch ROCm stack (torch 2.9.1+rocmsdk).

If your machine does not match, the installer shows the specs it found and offers to let you send them to us for review. It then exits without installing anything (exit code 10). Other hardware is not supported by this build.

## Download

Installer: `SeedVR2-AMD-Setup-1.1.0.exe` — 221,016 bytes
SHA-256: `82f0c5cff2805f5a5c418f4286eb5dc1f555c778474a62d4133a00138dc6bafd`

## We port NVIDIA software to AMD

Hi I'm Hal ports AI software that was made for NVIDIA only, so it runs on AMD hardware.

Got a program you'd like to see ported? Suggest it. And if your AMD machine isn't on our tested list, you can offer your specs for testing through our compatibility program.

Contact us at https://hiimhal.com

## Licence and credit

Licence: Apache License 2.0. SeedVR2 was created by ByteDance Seed; this port runs the open-source SeedVR2 implementation via ComfyUI.

Upstream projects: https://github.com/IceClear/SeedVR2 and https://github.com/Comfy-Org/ComfyUI — credit to their authors. This port is not affiliated with or endorsed by the upstream projects.

Ported by a developer from Ontario.
Home and full catalogue: https://hiimhal.com
Support: hello@hiimhal.com
