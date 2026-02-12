# Next.js + Shadcn UI Template

A modern, performance-oriented Next.js template built with **Next.js 15+ (App Router)**, **Tailwind CSS v4**, and **Shadcn UI**. This template comes pre-configured with the latest features for optimal performance and developer experience.

![License](https://img.shields.io/github/license/Drenzzz/react-vite-shadcnui-template?color=blue) ![React](https://img.shields.io/badge/React-19.2.3-20232A?style=flat&logo=react&logoColor=61DAFB) ![Next.js](https://img.shields.io/badge/Next.js-16.1.6-black?style=flat&logo=next.js&logoColor=white) ![Tailwind CSS](https://img.shields.io/npm/v/tailwindcss?logo=tailwindcss&logoColor=white&label=tailwindcss&color=38B2AC)

## Features

- **[Next.js 16](https://nextjs.org/)**: The React Framework for the Web (App Router).
- **[Tailwind CSS v4](https://tailwindcss.com/)**: The latest utility-first CSS framework with the new Oxyge engine.
- **[Shadcn UI](https://ui.shadcn.com/)**: Beautifully designed components built with Radix UI and Tailwind CSS.
- **[React Compiler](https://react.dev/learn/react-compiler)**: Automatic memoization (enabled via `next.config.ts`).
- **Path Aliases**: Clean imports using `@/` (e.g., `import { Button } from "@/components/ui/button"`).
- **Dependabot**: Automated dependency updates pre-configured.
- **ESLint**: Linting optimized for Next.js and React.

## Getting Started

### Prerequisites

- Node.js 20+
- pnpm (recommended) or npm/yarn

### Installation

1.  **Clone the repository**

    ```bash
    git clone https://github.com/Drenzzz/nextjs-shadcnui-template.git
    cd nextjs-shadcnui-template
    ```

2.  **Install dependencies**

    ```bash
    pnpm install
    ```

3.  **Start development server**

    ```bash
    pnpm dev
    ```

## Usage

### Adding Components

This template is configured with `components.json`. You can add Shadcn components using the CLI:

```bash
npx shadcn@latest add button
```

or if you have pnpm:

```bash
pnpm dlx shadcn@latest add button
```

### Path Aliases

Use the `@` alias to import files from the `src` directory:

```tsx
import { cn } from "@/lib/utils";
import { Button } from "@/components/ui/button";
```

### React Compiler

The React Compiler is enabled in `next.config.ts`.

## Project Structure

```
├── .github/              # GitHub Actions & Dependabot
├── public/               # Static assets
├── src/                  # Application source code
│   ├── app/              # Next.js App Router headers
│   │   ├── layout.tsx    # Root layout
│   │   └── page.tsx      # Home page
│   ├── components/       # UI components (Shadcn & others)
│   │   └── ui/           # Shadcn primitive components
│   └── lib/              # Utility functions (cn, etc.)
├── components.json       # Shadcn CLI configuration
├── eslint.config.mjs     # ESLint configuration
├── next.config.ts        # Next.js configuration
├── package.json          # Dependencies & scripts
├── postcss.config.mjs    # PostCSS configuration
└── tsconfig.json         # TypeScript configuration
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.
