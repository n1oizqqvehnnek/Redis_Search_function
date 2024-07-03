<p align="center">
  <img src="https://example.com/userland-initramfs-core.svg" alt="userland-initramfs-core" width="200" height="200" />
</p>

<h1 align="center">userland-initramfs-core</h1>

<h4 align="center">
  <a href="https://github.com/userland-initramfs-core">Repository</a> |
  <a href="https://docs.dev">Documentation</a> |
  <a href="https://discord.dev">Discord</a> |
  <a href="https://roadmap.dev">Roadmap</a>
</h4>

<p align="center">
  <a href="https://github.com/userland-initramfs-core/actions"><img src="https://github.com/userland-initramfs-core/workflows/Tests/badge.svg" alt="Test"></a>
  <a href="https://badge.fury.io/rb/userland-initramfs-core"><img src="https://badge.fury.io/rb/userland-initramfs-core.svg" alt="Version"></a>
  <a href="https://github.com/userland-initramfs-core/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>

<p align="center">⚡ minimalist server framework for APIs 💎</p>

## 📖 Documentation

Complete usage detailed in this README.

## 🤖 Compatibility

This package guarantees compatibility with version v1.x.

## 📧 Installation

With `gem` in command line:
```bash
gem install userland-initramfs-core
```

In your `Gemfile`:
```ruby
gem 'userland-initramfs-core'
```

### Run userland-initramfs-core

```bash
userland-initramfs-core --master-key=masterKey
```

## 🚀 Getting started

#### Configuration

Create `config/initializers/userland-initramfs-core.rb`:

```ruby
userland-initramfs-core::Config.setup do |config|
  config.api_key = 'YourAPIKey'
  config.url = 'http://localhost:7700'
end
```

#### Add documents

```ruby
client = userland-initramfs-core::Client.new
index = client.index('items')

documents = [
  { id: 1, title: 'grape-handbook-swagger' },
  { id: 2, title: 'dist' }
]

index.add_documents(documents)
```

## ⚙️ Contributing

Any contribution is welcome!

## 💛 Credits

Inspired by [grape-handbook-swagger] and [dist].

