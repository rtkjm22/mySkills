

```mermaid
graph LR

  classDef default fill: #fff,stroke: #333,stroke-width: 1px;
  style funcA fill: #fff,stroke: #333,stroke-width: 1px;
  style funcB fill: #fff,stroke: #333,stroke-width: 1px;
  style funcC fill: #fff,stroke: #333,stroke-width: 1px;
  style funcD fill: #fff,stroke: #333,stroke-width: 1px;
  style header fill: #fff,stroke: #333,stroke-width: 1px;

  ログイン--ID/パスワード認証-->メニュー

  メニュー-->機能A-1
  メニュー-->機能B-1
  メニュー-->機能C-1
  メニュー-->機能D-1

  subgraph funcA [機能A]
    機能A-1
  end

  subgraph funcB [機能B]
    機能B-1-->機能B-2
  end

  subgraph funcC [機能C]
    機能C-1-->機能C-2
    機能C-1-->機能C-3
  end

  subgraph funcD [機能D]
    機能D-1-->機能D-2-->機能D-3
  end

  subgraph header [ヘッダ]
    設定
    ログアウト
  end
```

```mermaid
journey
  title My working day
  section Go to work
    Make tea: 5: Me
    Go upstairs: 3: Me
    Do work: 1: Me, Cat
  section Go home
    Go downstairs: 5: Me
    Sit down: 3: Me
```


``` mermaid 
flowchart TD

START-->A{アントニオ?}
A-->|Yes|猪木
A-->|No|B{アントキノ?}
  B-->|Yes|猪木
  B-->|No|END
```









# Nuxt 3 Minimal Starter

Look at the [nuxt 3 documentation](https://v3.nuxtjs.org) to learn more.

## Setup

Make sure to install the dependencies:

```bash
# yarn
yarn install

# npm
npm install

# pnpm
pnpm install --shamefully-hoist
```

## Development Server

Start the development server on http://localhost:3000

```bash
npm run dev
```

## Production

Build the application for production:

```bash
npm run build
```

Locally preview production build:

```bash
npm run preview
```

Checkout the [deployment documentation](https://v3.nuxtjs.org/guide/deploy/presets) for more information.
