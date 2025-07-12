# VL.FLOSS

A vvvv wrapper for [FLOSS, the FLARE Obfuscated String Solver](https://github.com/mandiant/flare-floss). 
This library will give you a convenient `FLOSS` node that will let you run `floss.exe` from your patch and get the analysis results as a string.

## What is FLOSS?

As per FLOSS' repository README, "The FLARE Obfuscated String Solver (FLOSS, formerly FireEye Labs Obfuscated String Solver) uses advanced static analysis techniques to automatically extract and deobfuscate all strings from malware binaries. You can use it just like `strings.exe` to enhance the basic static analysis of unknown binaries."

In other words, it's `strings.exe` but better.

## Usage

In order to use this library, you'll have to donwnload `floss.exe` yourself. Clone this repository anywhere you'd like and create a `📂 /bin` folder next to `VL.FLOSS.vl`. Then, go to the [FLOSS repository's release page](https://github.com/mandiant/flare-floss/releases/latest), grab the latest Windows build and drop it in `/bin`. In the end, you should have something like

```
.
└── 📂 VL.FLOSS/
    ├── 📂 bin/
    │   └── ⚙️ floss.exe
    ├── 📂 help
    ├── 📄 .gitignore
    ├── 📄 README.MD
    └── ⬛ VL.FLOSS.vl
```

You can then check the help patch or drop the `FLOSS` node in a patch and hover its pins for more information.