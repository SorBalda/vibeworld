# VibeCity Mod SDK

Copyright 2026 Andrea Baldanza (the VibeCity project).

This directory is the home of the public VibeCity Mod SDK: the schemas,
host-API headers, example mod-packs, and any code explicitly published for
third parties to build and share mods against. Everything in this directory
is licensed under the **Apache License 2.0** (see [`LICENSE`](LICENSE)) —
intentionally permissive so anyone can create and distribute mods freely.

**Status:** the SDK has not been carved out into a separate module yet; this
directory currently holds only the legal base. Until then, the declarative
mod-pack format lives in `internal/modpack` and is covered by the client's
PolyForm Perimeter license (see the repository root [`LICENSE`](../LICENSE));
the Apache-2.0 license here applies only to material that is later explicitly
published as the Mod SDK.

Mods you write against the SDK are your own work: a mod is data validated
against Apache-licensed schemas, not a derivative of the VibeCity core.
