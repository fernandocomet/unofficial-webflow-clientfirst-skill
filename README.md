# Webflow Client-First Skill for Claude

An unofficial Claude skill for building Webflow projects using **Client-First** — the industry-standard naming convention and folder structure system by Finsweet.

> **Created by [Fernando Comet](https://fernandocomet.com)**. This skill helps Claude act as an expert developer in the Client-First methodology to ensure scalable, organized, and professional Webflow builds.

---

## What is Client-First?

Client-First is a set of guidelines and naming conventions for Webflow that prioritizes clear organization and scalability. It moves away from chaotic naming to a structured approach:

```
section-[identifier] → container-[size] → [identifier]_wrapper → [identifier]_component
```

By following this skill, Claude ensures that every class added to your project is logical, follows the official Finsweet folders, and remains maintainable for any client or team member.

---

## What this skill covers

- **Naming Convention** — Strict adherence to `folder-name_item` and `utility-class` structures.
- **Core Strategy** — Implementation of Strategy 1 (Custom) and Strategy 2 (Utility) based on project needs.
- **Global Styles** — Managing the `Style Guide` page and global typography/color variables.
- **Layout Structure** — Proper use of `page-wrapper`, `main-wrapper`, and `section-[name]`.
- **Component Workflow** — Creating "Components" with clear identifiers and nested elements.
- **Responsive Design** — Best practices for mobile-first or desktop-first scaling within the framework.
- **Spacing System** — Correct application of padding and margin utility classes.

---

## What works with the Webflow MCP

This skill is designed to be used alongside the official Webflow Model Context Protocol (MCP):

### ✅ Works well
- **Class Generation** — Claude can suggest perfect Client-First names for any element.
- **Structure Auditing** — Paste your HTML/DOM structure and Claude will fix non-compliant naming.
- **CMS Management** — Create collections and fields that follow the `blog_` or `team_` naming logic.
- **SEO & Settings** — Update page metadata and slugs directly via Claude.
- **Text Editing** — Update headings and paragraphs while maintaining class integrity.

### ⚠️ Known API limitations

1. **Class Creation** — The current Webflow MCP has limitations in creating *new* CSS classes directly; it is best used for generating the naming logic which you then apply in the Designer.
2. **Global Swatches** — Limited access to the color variable panel via API.
3. **Component Slots** — Not yet supported by the Webflow MCP, requiring manual placement for nested components.

---

## How to use

1. Add the `SKILL.md` file from this repository to your Claude Project or attach it to your conversation.
2. Ensure the [Webflow connector](https://webflow.com/blog/webflow-claude-connector) is active in your Claude environment.
3. Prompt Claude: *"I am building a 'Contact' section using Client-First. Suggest the structure and class names for a 3-column form."*

---

## Credits

- **Client-First Framework** created by [Finsweet](https://www.finsweet.com/client-first).
- **Claude Skill** developed by [Fernando Comet](https://fernandocomet.com).
- Built for use with [Claude](https://claude.ai) + [Webflow MCP](https://developers.webflow.com/mcp).

---

## Contributing

Suggestions to improve the expert prompts or tool definitions are welcome! Feel free to open a PR or an issue. As Finsweet updates the framework to v3+ or the Webflow MCP adds new features, this skill will be updated accordingly.
