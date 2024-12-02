<h1 align="center">
 <a href="https://x.com/MaindexAI">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="images/maindex-logo-dark"/>
    <source media="(prefers-color-scheme: light)" srcset="images/maindex-logo-light"/>
    <img width="400" src="images/maindex-logo-dark-bg.png"/>
 </a>
 <br />
</h1>
<br />

<div align="center">

<br>
<a href="https://x.com/MaindexAI">
  Twitter:@MaindexAI
</a>

</div>

<br>

<h3 align="center">AI driven development in your terminal.<br/>Build entire features and apps with a robust workflow.</h3>

<br/>
<br/>

## Learn more about Maindex  🧐

- [Overview](#overview-)
- [Install](#install)
- [Get started](#get-started-)
- [Build complex software](#build-complex-software-with-llms-)
- [Why Maindex?](#why-maindex-)
- [Roadmap](#roadmap-%EF%B8%8F)
- [Discussion and discord](#discussion-and-discord-)
- [Contributors](#contributors-)
<br/>

## Overview  📚

<p>Churn through your backlog, work with unfamiliar technologies, get unstuck, and <strong>spend less time on the boring stuff.</strong></p>

<p>Maindex is a <strong>reliable and developer-friendly</strong> AI coding agent in your terminal. It can plan out and complete <strong>large tasks</strong> that span many files and steps.</p>
 
<p>Designed for <strong>real-world use-cases</strong>, Maindex can help you build a new app quickly, add new features to an existing codebase, write tests and scripts, understand code, and fix bugs. </p>

<br/>

## Install  📥

```bash
curl -sL https://maindex.ai/install.sh | bash
```

**Note:** Windows is supported via [WSL](https://learn.microsoft.com/en-us/windows/wsl/install). Maindex only works correctly on Windows in the WSL shell. It doesn't work in the Windows CMD prompt or PowerShell.


<br/>

## Get started  🚀

Maindex uses OpenAI by default. If you don't have an OpenAI account, first [sign up here.](https://platform.openai.com/signup)

Then [generate an API key here](https://platform.openai.com/account/api-keys) and `export` it.

```bash
export OPENAI_API_KEY=...
```


Now `cd` into your **project's directory.** Make a new directory first with `mkdir your-project-dir` if you're starting on a new project.

```bash
cd your-project-dir
```


Then **start your first plan** with `maindex new`.

```bash
maindex new
```


Load any relevant files, directories, directory layouts, urls, or images **into the LLM's context** with `maindex load`.

```bash
maindex load some-file.ts another-file.ts
maindex load src/components -r # load a whole directory
maindex load src --tree # load a directory layout (file names only)
maindex load src/**/*.ts # load files matching a glob pattern
maindex load https://raw.githubusercontent.com/maindex-ai/maindex/main/README.md # load the text content of a url
maindex load images/mockup.png # load an image
```


Now **send your prompt.** You can pass it in as a file:

```bash
maindex tell -f prompt.txt
```


Write it in vim:

```bash
maindex tell # tell with no arguments opens vim so you can write your prompt there
```


Or pass it inline (use enter for line breaks):

```bash
maindex tell "add a new line chart showing the number of foobars over time to components/charts.tsx"
```

maindex will make a plan for your task and then implement that plan in code. **The changes won't yet be applied to your project files.** Instead, they'll accumulate in Maindex's sandbox.



<br/>

## Build complex software with LLMs  🌟

⚡️  Changes are accumulated in a protected sandbox so that you can review them before automatically applying them to your project files. Built-in version control allows you to easily go backwards and try a different approach. Branches allow you to try multiple approaches and compare the results.

📑  Manage context efficiently in the terminal. Easily add files or entire directories to context, and keep them updated automatically as you work so that models always have the latest state of your project.

🧠  By default, Maindex relies on the OpenAI API and requires an `OPENAI_API_KEY` environment variable. You can also use it with a wide range of other models, including Anthropic Claude, Google Gemini, Mixtral, Llama and many more via OpenRouter.ai, Together.ai, or any other OpenAI-compatible provider.

✅  Maindex supports Mac, Linux, FreeBSD, and Windows. It runs from a single binary with no dependencies.

<br/>

## Why Maindex?  🤔

🏗️  Go beyond autocomplete to build complex functionality with AI.<br>
🚫  Stop the mouse-centered, copy-pasting madness of coding with ChatGPT.<br>
⚡️  Ensure the model always has the latest versions of files in context.<br>
🪙  Retain granular control over what's in the model's context and how many tokens you're using.<br>
⏪  Rewind, iterate, and retry as needed until you get your prompt just right.<br>
🌱  Explore multiple approaches with branches.<br>
🔀  Run tasks in the background or work on multiple tasks in parallel.<br>
🎛️  Try different models and temperatures, then compare results.<br>

<br/>

## Roadmap  🗺️

🧠  Support for open source models, Google Gemini, and Anthropic Claude in addition to OpenAI  ✅ released<br>
🖼️  Support for multi-modal models—add images and screenshots to context ✅ released<br>
🤝  Plan sharing and team collaboration<br>
🖥️  VSCode and JetBrains extensions<br>
📦  Community plugins and modules<br>
🔌  Github integration<br>
🌐  Web dashboard and GUI<br>
🔐  SOC2 compliance<br>
🛩️  Fine-tuned models<br>

This list will grow and be prioritized based on your feedback.

<br/>

## Discussion and discord  💬

Speaking of feedback, feel free to give yours, ask questions, report a bug, or just hang out:

<br/>

## Contributors  👥

⭐️  Please star, fork, explore, and contribute to Maindex. There's a lot of work to do and so much that can be improved.

Work on tests, evals, prompts, and bug fixes is especially appreciated.



