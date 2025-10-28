# CodeVideo

![CodeVideo Logo](https://codevideo.io/logo.png)

## Educational Software Course and Content Creation, Reimagined

CodeVideo is an event-sourced IDE state manager that enables software educators and content creators to create professional educational content at unprecedented speed.

To read about the theory behind the framework, check out our [white paper](https://github.com/princefishthrower/codevideo-white-paper)

The framework is broken down into small parts, each with their own single responsibility:

Core Layer:

`codevideo-types` [![GitHub stars](https://img.shields.io/github/stars/codevideo/codevideo-types)](https://github.com/codevideo/codevideo-types/stargazers)

Virtual Layer (Sits on top of the core layer):

`codevideo-virtual-ide` [![GitHub stars](https://img.shields.io/github/stars/codevideo/codevideo-virtual-ide)](https://github.com/codevideo/codevideo-virtual-ide/stargazers)

`codevideo-virtual-file-explorer` [![GitHub stars](https://img.shields.io/github/stars/codevideo/codevideo-virtual-file-explorer)](https://github.com/codevideo/codevideo-virtual-file-explorer/stargazers)

`codevideo-virtual-editor` [![GitHub stars](https://img.shields.io/github/stars/codevideo/codevideo-virtual-editor)](https://github.com/codevideo/codevideo-virtual-editor/stargazers)

`codevideo-virtual-terminal` [![GitHub stars](https://img.shields.io/github/stars/codevideo/codevideo-virtual-terminal)](https://github.com/codevideo/codevideo-virtual-terminal/stargazers)

`codevideo-virtual-mouse` [![GitHub stars](https://img.shields.io/github/stars/codevideo/codevideo-virtual-mouse)](https://github.com/codevideo/codevideo-virtual-mouse/stargazers)

GUI Layer (Sits on top of the virtual layer):

`codevideo-ide-react` [![GitHub stars](https://img.shields.io/github/stars/codevideo/codevideo-ide-react)](https://github.com/codevideo/codevideo-ide-react/stargazers)

SaaS App Layer:

`codevideo-frontend` [![GitHub stars](https://img.shields.io/github/stars/codevideo/codevideo-frontend)](https://github.com/codevideo/codevideo-frontend/stargazers)

`codevideo-backend` [![GitHub stars](https://img.shields.io/github/stars/codevideo/codevideo-backend)](https://github.com/codevideo/codevideo-backend/stargazers)

`codevideo-api` [![GitHub stars](https://img.shields.io/github/stars/codevideo/codevideo-api)](https://github.com/codevideo/codevideo-api/stargazers)

Generators:

`codevideo-doc-gen` [![GitHub stars](https://img.shields.io/github/stars/codevideo/codevideo-virtual-ide)](https://github.com/codevideo/codevideo-doc-gen/stargazers)

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## 🚀 What is CodeVideo?

CodeVideo is a deterministic recording system that captures coding sessions as a series of discrete events. Rather than recording your screen as a video (with all the associated editing headaches), CodeVideo builds a timeline of interactions with your code editor, file system, and terminal.

## 🔍 How It Works (Technically)

1. **Action Definition**: Every action is defined using 
2. **Timeline Construction**: Events are organized into a deterministic timeline with edit capabilities.
3. **Generators**: The actions can be rendered in various output formats:
  - Video: each step is recorded as a video in parallel and stitched together
  - Markdown: generated via `codevideo-doc-gen`
  - HTML: generated using `marked`.
  - PDF: Currently, just a PDF format of the HTML, generated in the browser

## 🔌 IAction Interface

This simple two key-value JSON object forms the entire backbone of the CodeVideo framework:

```json
{
  "name": "editor-type",
  "value": "console.log('hello, world!');",
}
```

That's it! 

See the `IAction` interface from the [CodeVideo types repository](https://github.com/codevideo/codevideo-types) for more information.

## 📊 Performance Metrics

- **Export Speeds**: 
  - 5-minute tutorial to video: ~30 seconds
  - 5-minute tutorial to markdown: ~2 seconds

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

We welcome contributions from the community! Please check our [CONTRIBUTING.md](CONTRIBUTING.md) guide for details.
