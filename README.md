# PromptForge

> A beautiful, standalone web app for prompt engineers to build, organize, remix, and preview AI image generation prompts — equally powerful for **txt2img** and **img2img** workflows.

**Live Demo**: [Open the interactive UI demo](https://masterp001.github.io/PromptForge/) *(GitHub Pages enabled below)*

---

## 🎯 Project Vision

PromptForge is both a **production-ready prompt management tool** and a **design exploration playground** for the next generation of AI creative tooling.

It addresses the real pain points of prompt engineers:
- Fragmented prompts across chats, notes, and spreadsheets
- No easy way to version, remix, or A/B test variations
- Context loss when switching between txt2img and img2img
- Difficulty organizing hundreds of prompts with rich metadata

## ✨ Core Features (Implemented in Demo)

- **Modular Prompt Builder**: Drag-and-drop or click-to-add prompt blocks (subject, style, lighting, camera, negative, etc.)
- **Unified Library**: Browse/search hundreds of prompts with powerful filters (tags, model, type, collections)
- **Dual-Mode First-Class**: Seamless toggle or parallel views for txt2img ↔ img2img
- **Image Dropzone**: Upload reference image → auto-suggest or reuse compatible prompts
- **Variation Studio**: Generate/compare up to 6 side-by-side variations with one click (different seeds, slight remixes)
- **Collections & Tagging**: Organize into folders/collections, smart tags, favorites
- **Rich Metadata**: Full exposure of checkpoint, LoRAs, embeddings, sampler, steps, CFG, seed, negative prompt, thumbnails
- **Remix & Edit**: One-click remix, inline editing, history
- **Preview Gallery**: Masonry or grid of example outputs with hover details

## 🖼️ UI Design Concepts Explored

This repo contains multiple UI direction explorations. The main demo implements **Concept C: "IDE + Gallery Hybrid"** (detailed below). Other concepts are documented with high-fidelity descriptions and rationale.

### Concept A: "Creative Canvas" (Masonry + Floating Actions)
- **Vibe**: Artistic, fluid, inspiration-first (like Behance + Notion)
- **Layout**: Full-bleed masonry grid of prompt cards (thumbnail + title + tags + quick actions)
- **Interaction**: Hover reveals "Remix", "Add to Collection", "Compare"
- **Builder**: Floating "+ New Prompt" panel that expands into a beautiful block composer with live preview
- **Best for**: Visual prompt engineers who think in images first
- **Strengths**: High delight, quick browsing of large libraries
- **Trade-offs**: Less precise metadata editing on small screens

### Concept B: "Command Center" (Three-Panel IDE)
- **Vibe**: Pro tool, dark, dense, power-user (like VS Code + Figma)
- **Layout**: Left sidebar (Library + Collections + Search/Filters), Center (Prompt Editor + Block Palette), Right (Live Preview + Variations + Metadata)
- **Interaction**: Keyboard shortcuts everywhere, split-view for txt/img, drag blocks between panels
- **Best for**: Heavy daily users who want maximum information density and speed
- **Strengths**: Extremely efficient for power users, excellent for side-by-side comparison
- **Trade-offs**: Steeper learning curve, can feel overwhelming initially

### Concept C: "Hybrid Studio" (Current Demo)
- **Vibe**: Balanced modern + creative (clean dark theme with subtle neon accents, glassmorphism cards)
- **Layout**: Top nav (Library | Builder | Studio | Collections), Main area with resizable or tabbed sections
- **Key Screens**:
  - **Library View**: Searchable grid/list toggle + facet filters (model, tags, type, has image ref)
  - **Prompt Detail Modal**: Rich metadata, negative prompt, example gallery, one-click variations
  - **Builder**: Visual block system (chips for subject/style/quality/lighting/etc.) + full text editor + live token count
  - **Studio / Compare**: Drop image or select prompt → generate 6 variations in a beautiful comparison grid
- **Best for**: Most users — balances discoverability, editing power, and visual feedback
- **Why chosen as primary**: Excellent scalability to hundreds of prompts, works great on desktop (target), mobile-friendly with responsive collapse

### Concept D: "Minimal Zen" (Card + Focus Mode)
- **Vibe**: Calm, spacious, high-end product (like Linear or Arc browser)
- **Layout**: Large centered cards, generous whitespace, subtle animations
- **Interaction**: Command palette (⌘K) for everything, focus mode hides chrome when editing
- **Best for**: Users who get overwhelmed by too many options
- **Strengths**: Beautiful, low cognitive load
- **Trade-offs**: Slower for bulk actions

## 🛠️ Tech Stack (Demo)

- Pure HTML + Tailwind CSS (via CDN) + Vanilla JS
- Fully self-contained single-file demo (no build step)
- Ready for GitHub Pages or easy embedding
- Future: Can be extended to React/Next.js or Tauri desktop app

## 🚀 Getting Started

1. Clone the repo
2. Open `index.html` in browser (or enable GitHub Pages for live demo)
3. Explore the different tabs: **Library**, **Builder**, **Studio**

## 📸 Screenshots & Mockups

*(Screenshots of the live demo and concept wireframes will be added — or generate via the demo itself)*

## 🤝 Contributing

This is an open exploration! Feel free to fork, open issues with new UI ideas, or submit improved prompt block libraries.

**Prompt blocks included in demo**:
- Subject / Character
- Environment / Scene
- Lighting & Mood
- Camera & Composition
- Style & Artist References
- Technical Quality (masterpiece, best quality, etc.)
- Negative Prompt Blocks

## 📄 License

MIT — Use freely for your own prompt engineering tools.

---

*Built with ❤️ for the AI art community by Grok + Peter*  
*May 2026*