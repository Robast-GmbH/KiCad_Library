# KiCad_Library
This repository contains our KiCad symbol librariy with atomic parts.
It is inspired by [kicad-library](https://github.com/OpenCleanEnergy/kicad-library) and is using the [KiCad-Db-Lib](https://github.com/Projektanker/kicad-db-lib).

## Add KiCad Symbols

1. Add remote
```bash
git remote add -f kicad-symbols https://gitlab.com/kicad/libraries/kicad-symbols.git
```

2. Add the subtree (check your KiCad Version and insert correct `KICAD_VERSION`, at the time of writing this is `v7`)
```bash
git subtree add --prefix symbols kicad-symbols KICAD_VERSION --squash
```

## Add KiCad Footprints

1. Add remote
```bash
git remote add -f kicad-footprints https://gitlab.com/kicad/libraries/kicad-footprints.git
```

2. Add the subtree (check your KiCad Version and insert correct `KICAD_VERSION`, at the time of writing this is `v7`)
```bash
git subtree add --prefix footprints kicad-footprints KICAD_VERSION --squash
```

## Add KiCad 3D packages

1. Add remote
```bash
git remote add -f kicad-packages3D https://gitlab.com/kicad/libraries/kicad-packages3D.git
```

2. Add the subtree
```bash
git subtree add --prefix packages3D kicad-packages3D master --squash
```

## Update KiCad Symbols, Footprints or 3D packages

### Symbols (check your KiCad Version and insert correct `KICAD_VERSION`, at the time of writing this is `v7`)
```bash
git subtree pull --prefix symbols kicad-symbols KICAD_VERSION --squash
```

### Footprints (check your KiCad Version and insert correct `KICAD_VERSION`, at the time of writing this is `v7`)
```bash
git subtree pull --prefix footprints kicad-footprints KICAD_VERSION --squash
```

### 3D packages
```bash
git subtree pull --prefix kicad-packages3D kicad-kicad-packages3D master --squash
```