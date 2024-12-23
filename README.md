<div align="center">

# rails.nvim

A lightweight Neovim plugin that adds a :Rails command for easy access to Artisan and Composer tasks.

**Shoutout to Claude for adapting [laravel.nvim](https://github.com/djaruun/laravel.nvim) for Rails and rewriting it in Lua!**

</div>

## ⚡ Requirements

- Neovim 0.8+

## 📦 Installation

rails.nvim supports all the usual plugin managers

<details open>
  <summary><a href="https://github.com/folke/lazy.nvim">🔗</a> lazy.nvim</summary>

```lua
{
  "djaruun/rails.nvim",
  config = true,
}
```
</details>

## 🔌 Quick start

<details>
<summary>Full config example for lazy.nvim</summary>

```lua
{
  "djaruun/rails.nvim",
  config = true,
}
```
</details>

## 🚀 Usage

In Rails projects, do `:Rails` and then your favorite Rails command.

#### Example of starting the dev server using bin/dev:

`:Rails dev`

#### The same example using the regular rails server:

`:Rails server`

#### Example of running database migrations:

`:Rails db:migrate`

## 🔧 Configuration

At the moment there is no configuration options available. It should just work out of the box.
If there are any options you would like or it doesn't work like it should, please feel free open an issue in the repository!

## ⚙️ Technical overview

Basically, all it does is run `term bin/rails <command>` for you and generates command completions from the available commands from the Rails CLI using `bin/rails -h`.

## 💫 Star History

[![Star History Chart](https://api.star-history.com/svg?repos=djaruun/rails.nvim&type=Date&theme=dark)](https://star-history.com/#djaruun/rails.nvim&Date)
