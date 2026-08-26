# All The Fabric 3

All The Fabric 3, version V6, for Minecraft 1.18.2 on Fabric 0.14.10, laid out
as a portable pack the LANMinecraft launcher can install and update.

The tree is the CurseForge release: its manifest names 94 mods by project and
file id, and every one of them was fetched and checked against the SHA-1
CurseForge records for it, so what is here is what the authors published. The
`config/`, `journeymap/` and `simple-rpc/` trees come from the same archive.

`portable-pack.json` is what the launcher reads. A push to `main` regenerates
`pack-manifest.json` and refreshes the rolling `pack-latest` release the
launcher syncs from.

## Why this pack

It is the small one. Ninety-four mods and 255 MiB of them against All the Mods
10's four hundred and 1.3 GB, on a Minecraft that was lighter to begin with -
which is what makes it the pack a laptop with eight gigabytes can actually
hold. Its own performance base is already there: Sodium with Sodium Extra and
Reese's options, Lithium, Phosphor, Indium and MemoryLeakFix all ship with it.

## The generator was taught two folders

`journeymap/` and `simple-rpc/` are read by their mods directly and arrive in
the pack's own overrides, and the shared `tools/generate_manifest.py` knew
neither. A root outside its scan list is not merely left out of the manifest:
the launcher holds a pack folder to exactly what the manifest names and deletes
the rest, so both would have been swept away with nothing to say why.

Credit for the pack belongs to the All the Mods team, and to the author of every
mod in `mods/`.
