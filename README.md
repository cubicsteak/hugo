# Hugo Starter Blog - A Hugo Theme

`Hugo Starter Blog` is a minimal and clean blog theme for Hugo.

## Installation & Usage

This guide assumes you have Hugo installed on your machine. Follow the commands below to create a new Hugo site with the `Hugo Starter Blog` theme.

### 1. Create a New Hugo Site

Create a new site named `my-awesome-blog` and navigate into it.

```bash
hugo new site my-awesome-blog
cd my-awesome-blog

```

### 2. Initialize Git Repository

It is recommended to manage Hugo themes as Git submodules.

```bash
git init
```

### 3. Add `Hugo Starter Blog` Theme

You can install the theme using **Git Submodules** or **Hugo Modules**.

#### Option 1: Git Submodule (Recommended for simple setups)

You can bring the theme into a specific folder name (e.g., `hugo-starter-blog`).

```bash
git submodule add https://github.com/cubicsteak/hugo.git themes/hugo-starter-blog
```

#### Option 2: Hugo Modules (Modern approach)

If you prefer not to use submodules, you can use Hugo Modules.

```bash
# 1. Initialize hugo modules
hugo mod init github.com/yourusername/my-awesome-blog

# 2. Add the theme to your project
hugo mod get github.com/cubicsteak/hugo

# 3. Tidy up the modules
hugo mod tidy
```

### 4. Configure Theme

Open your configuration file (`hugo.toml` or `config.toml`) and set the `theme` parameter.

**If using Git Submodule:**

```toml
# hugo.toml
theme = "hugo-starter-blog"
```

**If using Hugo Modules:**

```toml
# hugo.toml
[module]
  [[module.imports]]
    path = "github.com/cubicsteak/hugo"
```

### 5. Create Your First Post

Generate a new markdown file for your post.

```bash
hugo new content posts/my-first-post.md
```

### 6. Run Local Server

Start the Hugo server to preview your site. The `-D` flag includes draft content.

```bash
hugo server -D
```


## Theme Information
* **Name:** Hugo Starter Blog
* **Description:** A minimal, responsive starter blog theme.
* **Author:** Brad ([@cubicsteak](https://github.com/cubicsteak))
* **Homepage:** [https://github.com/cubicsteak/hugo](https://github.com/cubicsteak/hugo)
* **License:** MIT
* **Tags:** `starter`, `blog`, `minimal`, `responsive`, `bootstrap`
