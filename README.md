# CWI World Desktop — Downloads

Windows portable builds of **CWI World Desktop 2.0.3** and **CWI Command Deck 1.0.0**.

## How this repo works

The zips are too large to upload in one shot from the build machine, so they are
stored here as 25 MB chunks under `chunks/`:

- `wd203.part.000` … `wd203.part.006` → `CWI World Desktop-2.0.3-win-portable.zip`
- `cd100.part.000` … `cd100.part.007` → `CWI Command Deck-1.0.0-win-portable.zip`

The **Assemble Windows builds and publish release** workflow (`Actions` tab →
`Run workflow`) concatenates the chunks, integrity-checks the zips, and publishes
them as downloadable assets on a GitHub Release. One link, no reassembly needed
on the download side.
