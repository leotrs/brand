# Aris Brand Assets

This repository contains all official brand assets for the Aris ecosystem. All Aris
projects should include this repository as a git submodule to ensure consistent
branding.

## Repository Structure

```
brand/
├── logos/
│   ├── aris/           # Main Aris brand logos
│   ├── studio/         # RSM Studio logos and favicons
│   ├── press/          # Preview Press logos
│   ├── forum/          # Aris Forum logos
│   └── rsm/            # RSM Python package logos
├── design-system/
│   ├── css/            # Design system CSS variables
│   └── README.md       # Design system documentation
├── colors/             # Color palette definitions (future)
└── typography/         # Typography specifications (future)
```

## Logo Variants

Each product has consistent logo variants:

- **Logotype**: Full horizontal logo (logomark + text)
- **Stacked**: Vertical layout (logomark above text)
- **Logomark**: Icon/symbol only
- **Grayscale**: Monochrome variant
- **App Icon**: High-resolution square icon (512px+)


## Export Specifications

When exporting new logos from Figma, use these specifications for consistency:

### Standard Sizes
- **Logotype (horizontal)**: 128px or 256px width (height auto)
- **Stacked (vertical)**: 128px or 256px height (width auto)
- **Logomark only**: 64px × 64px (square)
- **App icon**: 512px × 512px (for favicons/PWA icons)
- **Grayscale variants**: Same dimensions as color counterparts

### Export Settings
1. Use **frames** with exact locked dimensions in Figma
2. Export **all variants for all brands at once** from the same file
3. Use consistent export settings:
   - Format: SVG
   - Outline text: Enabled
   - Simplify stroke: Enabled
4. Naming convention: `{product}-{variant}-{size}.svg`
   - Examples: `aris-logo-64.svg`, `studio-logotype-256.svg`

## Design System

The `design-system/` directory contains CSS variables and design tokens used across Aris products. See `design-system/README.md` for details.

## Guidelines

### Usage Rules
- Always use logos from this repository (via submodule)
- Never modify logo files in individual projects
- Maintain aspect ratios when scaling
- Use appropriate variants for different contexts
- Follow spacing and clear space guidelines

### Color Palette
- **Aris**: Slate gray (#6B7280)
- **Studio**: Blue (#3B82F6)
- **Press**: Red/Coral (#EF4444)
- **Forum**: Purple (#A855F7)
- **RSM**: (see rsm/logo.svg for current colors)

## Contributing

To update brand assets:

1. Export new assets from Figma following the specifications above
2. Place files in appropriate directories
3. Update this README if adding new variants
4. Commit with descriptive message
5. All projects using this submodule will need to update their submodule reference

## License

All brand assets are proprietary to the Aris project. Use only for official Aris products and communications.
