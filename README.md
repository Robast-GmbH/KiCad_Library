# KiCad_Library
This repository contains our KiCad symbol librariy with atomic parts.
# KiCad_Library
This repository contains our KiCad symbol librariy with atomic parts.
It is inspired by: [kicad-library](https://github.com/OpenCleanEnergy/kicad-library)

## Add KiCad Symbols

1. Add remote
```bash
git remote add -f kicad-symbols https://gitlab.com/kicad/libraries/kicad-symbols.git
```

2. Add the subtree
```bash
git subtree add --prefix symbols kicad-symbols master --squash
```

## Add KiCad Footprints

1. Add remote
```bash
git remote add -f kicad-footprints https://gitlab.com/kicad/libraries/kicad-footprints.git
```

2. Add the subtree
```bash
git subtree add --prefix footprints kicad-footprints master --squash
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

### Symbols
```bash
git subtree pull --prefix symbols kicad-symbols master --squash
```

### Footprints
```bash
git subtree pull --prefix footprints kicad-footprints master --squash
```

### 3D packages
```bash
git subtree pull --prefix kicad-packages3D kicad-kicad-packages3D master --squash
```