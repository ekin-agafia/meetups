<p align="center">
  <img src="https://example.com/models_dbtool.svg" alt="models_dbtool" width="200" height="200" />
</p>

<h1 align="center">models_dbtool</h1>

<h4 align="center">
  <a href="https://github.com/models_dbtool">Repository</a> |
  <a href="https://docs.io">Documentation</a> |
  <a href="https://discord.io">Discord</a> |
  <a href="https://roadmap.io">Roadmap</a>
</h4>

<p align="center">
  <a href="https://github.com/models_dbtool/actions"><img src="https://github.com/models_dbtool/workflows/Tests/badge.svg" alt="Test"></a>
  <a href="https://badge.fury.io/rb/models_dbtool"><img src="https://badge.fury.io/rb/models_dbtool.svg" alt="Version"></a>
  <a href="https://github.com/models_dbtool/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>

<p align="center">⚡ minimalist server framework for APIs 💎</p>

## 📖 Documentation

Complete usage detailed in this README.

## 🤖 Compatibility

This package guarantees compatibility with version v1.x.

## 📧 Installation

With `gem` in command line:
```bash
gem install models_dbtool
```

In your `Gemfile`:
```ruby
gem 'models_dbtool'
```

### Run models_dbtool

```bash
models_dbtool --master-key=masterKey
```

## 🚀 Getting started

#### Configuration

Create `config/initializers/models_dbtool.rb`:

```ruby
models_dbtool::Config.setup do |config|
  config.api_key = 'YourAPIKey'
  config.url = 'http://localhost:7700'
end
```

#### Add documents

```ruby
client = models_dbtool::Client.new
index = client.index('items')

documents = [
  { id: 1, title: 'aws-s3' },
  { id: 2, title: 'CHANGELOG.md' }
]

index.add_documents(documents)
```

## ⚙️ Contributing

Any contribution is welcome!

## 💛 Credits

Inspired by [aws-s3] and [CHANGELOG.md].

