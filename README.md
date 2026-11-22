# Embercat

Industrial intelligence and smart asset monitoring suite.

Embercat is planned to bring together operations visibility, incidents and alerts, and an asset registry.

## Project status

This repository currently contains project documentation. The exported screen code, styles, images, design tokens, and master specification still need to be added before the website can be deployed.

## Planned screens

- Operations Overview
- Incidents & Alerts
- Asset Registry

## Recommended structure

```text
.
├── README.md
├── index.html              # Homepage to add
├── src/
│   ├── screens/            # Exported screen HTML, CSS, and JavaScript
│   └── slides/             # Presentation assets, if applicable
├── design-system/
│   ├── tokens.json         # Design tokens to add
│   └── tokens.css          # CSS tokens to add
└── docs/
    └── MASTER_SPEC.md      # Project specification to add
```

The structure above is a guide; the application files have not yet been committed. Keep asset paths valid when arranging the exported files.

## Add the website files

1. Export the Embercat screen code and assets from Stitch.
2. Add the files to this repository, including an `index.html` at the repository root.
3. Add the design tokens and specification to their respective folders.
4. Commit and push the changes to `main`.

For a local checkout:

```bash
git clone https://github.com/Mekala07/SmartAssetMonitoring.git
cd SmartAssetMonitoring

# Copy your exported website files into this folder, then:
git add .
git commit -m "feat: Add Embercat website files"
git push origin main
```

## Deploy to Vercel

After the website files have been committed:

1. Open [Vercel New Project](https://vercel.com/new) and sign in with GitHub.
2. Grant Vercel access to `Mekala07/SmartAssetMonitoring`.
3. Import the repository and use `embercat` as the project name, if available.
4. For a plain HTML, CSS, and JavaScript export, use:

   | Setting | Value |
   | --- | --- |
   | Framework Preset | Other |
   | Root Directory | Repository root (`./`) |
   | Build Command | Empty |
   | Output Directory | `.` |

5. Click **Deploy** and open the URL Vercel provides.

These settings assume the homepage is at the repository root and the site requires no build step. If the exported application uses a framework, use its corresponding Vercel preset and build settings instead.

Vercel can automatically deploy subsequent pushes to the connected production branch.

See [Vercel Git deployments](https://vercel.com/docs/git) and [build configuration](https://vercel.com/docs/builds/configure-a-build).

## Project name

The product name is **Embercat**. The GitHub repository is currently named **SmartAssetMonitoring**.
