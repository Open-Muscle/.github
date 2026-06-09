# Contributing to OpenMuscle

Thanks for helping build OpenMuscle, an open-source, modular prosthetic sensing
platform. This guide applies to **every repository in the
[Open-Muscle](https://github.com/Open-Muscle) organization**. It lives in the
org-wide `.github` repo, so any repo without its own `CONTRIBUTING.md`
automatically uses this one.

Contributions of every size are welcome: code, hardware design files, firmware,
documentation, test data, and ideas. You do not need to write code to
contribute, and you will be credited either way (see
[Credit and attribution](#credit-and-attribution)).

---

## Where things live

OpenMuscle is split into one repo per device or concern. File issues and pull
requests on the repo that owns the work.

| Area | Repository | What belongs here |
|------|-----------|-------------------|
| Hub / landing / cross-repo coordination | [OpenMuscle-Hub](https://github.com/Open-Muscle/OpenMuscle-Hub) | Project-wide questions, where-does-this-go questions, documentation index |
| FlexGrid hardware | [OpenMuscle-FlexGrid](https://github.com/Open-Muscle/OpenMuscle-FlexGrid) | Flexible + rigid PCB, BOM, schematics, enclosures |
| FlexGrid firmware | [FlexGridV3-Firmware](https://github.com/Open-Muscle/FlexGridV3-Firmware) | MicroPython firmware for the FlexGrid controller |
| LASK5 labeler | [OpenMuscle-LASK5](https://github.com/Open-Muscle/OpenMuscle-LASK5) | Handheld labeler wand hardware and docs |
| Shared software / pipeline | [OpenMuscle-Software](https://github.com/Open-Muscle/OpenMuscle-Software) | PC tooling, ML pipeline, shared firmware |
| AR / XR | [OpenMuscle-AR](https://github.com/Open-Muscle/OpenMuscle-AR) | WebXR client, future native headset app |
| Shared KiCad / CAD parts | [OpenMuscle-Library](https://github.com/Open-Muscle/OpenMuscle-Library) | Symbols, footprints, 3D models, mechanical parts shared across devices |
| Band (legacy) | [OpenMuscle-Band](https://github.com/Open-Muscle/OpenMuscle-Band) | Original 12-sensor armband |

Not sure which repo? Open an issue on the
[Hub](https://github.com/Open-Muscle/OpenMuscle-Hub/issues) and a maintainer
will route it.

---

## How to contribute

### 1. Open an issue first

Before writing code, open an issue on the repo that owns the work. This is true
for bugs, features, and ideas. It lets a maintainer confirm direction, avoids
duplicate effort, and creates the record that ties your idea to the eventual
change.

Use the issue forms when you open one:

- **Bug report** for something that is broken.
- **Feature request** for a concrete change you want built.
- **Idea / discussion** for a direction, concept, or open question that is not
  yet a specific change.

Idea-only issues are first-class. If all you have is a good idea, file it; you do
not have to implement it to be credited.

### 2. Discuss and scope

A maintainer triages the issue, applies labels, and works with you to scope it.
Issues that are ready to build get a `ready` label and, where useful, a
`good first issue` label for newcomers.

### 3. Open a pull request

When an issue is ready, work lands as a pull request **against the specific repo
the change belongs to** (not the Hub). In the PR description:

- Link the originating issue with a closing keyword, for example
  `Closes Open-Muscle/OpenMuscle-FlexGrid#42`.
- If the idea came from someone else, credit them (see below).
- Describe what changed and how you tested it. For hardware, note which board
  revision and which files (schematic, PCB, BOM) changed.

### 4. Review and merge

A maintainer reviews for correctness, scope, and licensing. Hardware changes are
reviewed against the existing board revision and BOM; firmware against the target
device. Once approved, the maintainer merges and the issue closes through its
linked keyword.

---

## Credit and attribution

Nobody who helps should go uncredited, including people whose only contribution
was an idea. OpenMuscle uses four overlapping mechanisms:

1. **Contributors graph.** Anyone whose pull request merges appears
   automatically in the repo's GitHub contributors graph.
2. **`CONTRIBUTORS.md`.** Idea-only and non-commit contributions are recorded in
   [CONTRIBUTORS.md](./CONTRIBUTORS.md) by hand. If you suggested something that
   shipped and you never pushed a commit, you belong on that list. Add yourself
   in your PR, or ask a maintainer to add you.
3. **Co-author trailers.** When one person implements another person's idea, the
   commit credits the originator with a Git trailer:

   ```
   Co-Authored-By: Real Name <email@example.com>
   ```

   GitHub then attributes the commit to both people.
4. **Issue and changelog links.** Every PR links its originating issue, so the
   trail from idea to merged code stays visible in the history.

---

## Licensing of contributions

Each repo declares its own license. By contributing, you agree your contribution
is licensed under that repo's license. The common cases:

- **Hardware** repos use **CERN-OHL-S-2.0**.
- **Firmware** repos use **MIT**.
- **Documentation** is generally **CC BY-SA 4.0**.

Check the `LICENSE` file in the specific repo before contributing. If you are
importing third-party files, make sure their license is compatible and note it
in your PR.

---

## Code of conduct

Participation in OpenMuscle is governed by the
[Code of Conduct](./CODE_OF_CONDUCT.md). Be respectful, assume good faith, and
help keep this a welcoming place for newcomers.

---

## Questions

Open an issue on the [Hub](https://github.com/Open-Muscle/OpenMuscle-Hub/issues)
or start a GitHub Discussion. Beginners are welcome; there is no question too
small.
