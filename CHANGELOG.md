# Changelog

All notable changes to **Rox UI**. Format loosely follows Keep a Changelog.

## [0.5.1]
### Added
- **`rox.css`** — single compiled stylesheet (no `@import`); drop in with one `<link>` and use the kit's styling without a bundler. Exposed as the `rox-ui/rox.css` export.
- This changelog.

## [0.5.0] — all 20 brainstorm improvements landed
### Added
- **Light + high-contrast themes** — `ColorThemeProvider`, `useColorTheme`, `ColorThemeSwitch` (`data-sf-theme` = `dark | light | hc`), persisted.
- **Scroll choreography** — `ScrollProgress` bar, `ScrollSignal` thread, and magnetic active-nav via `useActiveSection`.
- **cva variant API** — `Surface` (variant/tone/density) and `Button` (variant/tone/size) + `cn()` util.
- **Semantic glow** hover utilities (`.sf-glow-*`) and **container-query** utilities (`.sf-cq`, `.sf-cq-title`).
- **Opt-in sound** — `useStateSound` + `SoundToggle` (off by default, reduced-motion + SSR/jsdom safe).
- **Quality** — axe a11y test (0 violations); Ladle catalog (config + provider + stories); Playwright visual config/spec; ESLint flat + Prettier config; GitHub Actions CI.
### Changed
- `StateFirstPage` wires themes, scroll, sound, and active nav.
- 30 tests passing (was 20); typecheck clean incl. stories.

## [0.4.0] — quick-win polish
### Added
- Lit edges + `.sf-elev-1..3`, hero-stage gradient ring, filled-button highlight.
- Film grain on tinted panels (`prefers-reduced-data` aware).
- Tabular numerals on metrics/timestamps; reading measure + balanced headlines.
- Scoped `:focus-visible` ring (`--sf-focus`).
- Brand aliases: `--rox-*` CSS vars + `roxColors`/`roxSpring`/`roxEase`.

## [0.3.0] — glass + type scale
### Added
- Glass/translucency system (`--sf-glass-*`, `.sf-glass*`, `.sf-ring`), applied to nav/stage/cards.
- Modular type scale (`--sf-text-2xs..5xl`) + tracking/leading tokens + `.sf-t-*`.
- Rebrand to **Rox UI** (`rox-ui`), MIT license, PRD + brainstorm docs.

## [0.2.0] — library hardening
### Added / Fixed
- CSS-class architecture (restores hover/responsive fidelity); `MotionProvider` single source of truth; all 50 scenes; `StateFirstPage`; scene registry; tests.
