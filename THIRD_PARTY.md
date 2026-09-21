# Bundled third-party components

The complete Windows package includes unmodified official CPython 3.13.12 for Windows x64
from the Python Software Foundation NuGet package and pinned PyPI binary wheels.
These components retain their own copyrights and licenses. First-party PCS code is
licensed under GNU GPL version 3 only; see LICENSE and COPYRIGHT. This inventory
does not relicense third-party code, models, or runtime libraries. No SQLCipher or
custom CPython build is used.

Python source distribution: https://www.python.org/downloads/release/python-31312/
Runtime package: https://www.nuget.org/packages/python/3.13.12
Original package URL: https://api.nuget.org/v3-flatcontainer/python/3.13.12/python.3.13.12.nupkg
The ZIP is that original package with a .zip extension. Its SHA256 is
389c0228afbb3530f6cd079f5cec44139b1441dd51c85ec704f7a63f1c9f3802.

third-party/components.json records every bundled wheel, hash, declared license,
upstream metadata links, and version. Full bundled license/notice files are copied
under third-party/ and also retained inside the unmodified wheels/runtime archive.
cryptography uses its standard wheel with the upstream bundled cryptographic
libraries and their notices. This inventory is not a security audit.


## Offline speech recognition

Whisper.cpp b5130 (1.9.4), Windows x64 CPU build, and the Whisper base.en model are bundled in pcs/local_voice. Both use the MIT license; full notices are pcs/local_voice/whisper-LICENSE and pcs/local_voice/model-LICENSE. Runtime source: https://github.com/ggml-org/whisper.cpp/tree/b5130 . Model conversion: https://huggingface.co/ggerganov/whisper.cpp/tree/5359861c739e955e79d9a303bcbc70fb988958b1 . The pinned per-file hashes are in pcs/local_voice_manifest.json. Recognition is CPU-only and offline; no audio is written to a recording file.

Microsoft Visual C++ Runtime 14.44.35211 x64: msvcp140.dll, vcomp140.dll, vcruntime140.dll and vcruntime140_1.dll are included beside the speech executable. Copyright Microsoft Corporation. The Microsoft license is included at pcs/local_voice/microsoft-runtime-LICENSE.rtf. Source: https://aka.ms/vs/17/release/vc_redist.x64.exe . These app-local libraries do not install or replace the Windows runtime.
