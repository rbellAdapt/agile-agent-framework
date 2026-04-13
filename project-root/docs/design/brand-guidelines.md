# Acme E-Commerce Brand & Identity Guide

**Custodian:** `@brand`
**Version:** 1.0.0

This document serves as the single source of truth for the visual and tonal identity of the Acme E-Commerce Dashboard. All UI/UX implementations must adhere to these guidelines to ensure a professional, data-driven aesthetic is maintained.

---

## 1. The Core Aesthetic
- **Concept:** "Modern E-Commerce", Clean SaaS Interface.
- **Vibe:** Trustworthy, accessible, and highly performant.
- **Imagery:** "Metrics-forward" (e.g., stylized line charts, inventory grids, global fulfillment maps) with a secondary focus on positive vendor interactions.

---

## 2. Visual Identity & Color Palette

The color system is explicitly designed for a clean, professional dashboard environment that prioritizes high readability for financial metrics.

| Name | Hex Code | Tailwind Variable | Usage |
| :--- | :--- | :--- | :--- |
| **Pristine White (Background)** | `#ffffff` | `var(--background)` | Primary background color for all pages and components. |
| **Charcoal Gray (Foreground)** | `#1f2937` | `var(--foreground)` | Primary body text and general borders. High readability. |
| **Acme Blue (Accent)** | `#2563eb` | `var(--color-primary)` | Primary accent. Used in data plots, focused states, and primary CTAs. |
| **Growth Green (Accent)** | `#10b981` | `var(--color-success)` | Secondary accent. Used for positive financial metrics, success alerts, and highlights. |

> **@dev Note:** Ensure all primary text passes standard WCAG contrast ratios against the background. Keep charts colorblind-accessible.

---

## 3. Typography

Fonts must balance modern elegance with legibility for dense financial data.

### Sans-Serif (Body & UI)
- **Font Family:** `Inter` (Google Font)
- **Tailwind Variable:** `var(--font-inter)` / `font-sans`
- **Usage:** Standard body paragraphs, standard labels, and general navigation elements.

### Monospace (Data & Headers)
- **Font Family:** `Roboto Mono` (Google Font)
- **Tailwind Variable:** `var(--font-roboto-mono)` / `font-mono`
- **Usage:** Numerical real-time readouts, financial figures, data table headers, and SKU codes.

---

## 4. Copywriting & Tone of Voice

### The Persona
- You are a trusted enterprise platform speaking to business owners and logistics managers.
- **Tone:** Professional, precise, accessible, and direct. 

### Key Copy Rules
- **Focus on Actionable Data:** Highlight fulfillment times, inventory turnover, and clear sales metrics.
- **Action-Oriented:** Use verbs that denote business optimization (e.g., "Manage," "Analyze," "Forecast").
- **Clear and Simple:** Let the data guide the user. Avoid overly technical jargon when plain business language will suffice.

### Example Copy
- **Avoid:** "Our revolutionary synergistic data matrix makes your numbers better."
- **Use:** "The aggregated analytics view reduces weekly reporting time by an average of 4 hours."

---

## 5. UI/UX Principles (The "Feel")

- **Geometry:** Smooth, modern edges. Prefer subtle border radii like `rounded-md` or `rounded-lg` for cards and buttons.
- **Spacing:** Use generous, breathable padding and margins to make dense financial data easy to scan.
- **Motion:** Transitions should be smooth and helpful, using standard ease-out curves to guide the eye without feeling distracting.

---

> **VIBE CHECK REQUIREMENT:** All new frontend components submitted by `@dev` must be audited against this document using the mandatory Brand Audit checklist (see `/docs/.agents/skills/brand/SKILL.md`).
