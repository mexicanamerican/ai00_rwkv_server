# 💯AI00 RWKV Server

<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section --> 
[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-) 
<!-- ALL-CONTRIBUTORS-BADGE:END -->

`AI00 RWKV Server` is an inference API server based on the [`RWKV` model](https://github.com/BlinkDL/ChatRWKV).

It supports `VULKAN` inference acceleration and can run on all GPUs that support `VULKAN`. No need for Nvidia cards!!! AMD cards and even integrated graphics can be accelerated!!!

No need for bulky `pytorch`, `CUDA` and other runtime environments, it's compact and ready to use out of the box!

Compatible with OpenAI's ChatGPT API interface.

100% open source and commercially usable, under the MIT license.

If you are looking for a fast, efficient, and easy-to-use LLM API server, then `AI00 RWKV Server` is your best choice. It can be used for various tasks, including chatbots, text generation, translation, and Q&A.

Join the `AI00 RWKV Server` community now and experience the charm of AI!

QQ Group for communication: 30920262

### 💥Features

*   Based on the `RWKV` model, it has high performance and accuracy
*   Supports `VULKAN` inference acceleration, you can enjoy GPU acceleration without the need for `CUDA`! Supports AMD cards, integrated graphics, and all GPUs that support `VULKAN`
*   No need for bulky `pytorch`, `CUDA` and other runtime environments, it's compact and ready to use out of the box!
*   Compatible with OpenAI's ChatGPT API interface

### ⭕Usages

*   Chatbots
*   Text generation
*   Translation
*   Q&A
*   Any other tasks that LLM can do

### 👻Other

*   Based on the [web-rwkv](https://github.com/cryscan/web-rwkv) project
*   [Model download](https://huggingface.co/cgisky/RWKV-safetensors-fp16)

## Installation, Compilation, and Usage

### 📦Direct Download and Installation

1.  Directly download the latest version from [Release](https://github.com/cgisky1980/ai00_rwkv_server/releases)
    
2.  After [downloading the model](https://huggingface.co/cgisky/RWKV-safetensors-fp16), place the model in the `assets/models/` path, for example, `assets/models/RWKV-4-World-0.4B-v1-20230529-ctx4096.st`
    
3.  Run in the command line
    
    ```bash
    $ ./ai00_rwkv_server --model assets/models/RWKV-4-World-0.4B-v1-20230529-ctx4096.st
    ```
    
4.  Open the browser and visit the WebUI [`http://127.0.0.1:3000`](http://127.0.0.1:3000)
    

### 📜Compile from Source Code

1.  [Install Rust](https://www.rust-lang.org/)
    
2.  Clone this repository
    
    ```bash
    $ git clone https://github.com/cgisky1980/ai00_rwkv_server.git $ cd ai00_rwkv_server
    ```
    
3.  After [downloading the model](https://huggingface.co/cgisky/RWKV-safetensors-fp16), place the model in the `assets/models/` path, for example, `assets/models/RWKV-4-World-0.4B-v1-20230529-ctx4096.st`
    
4.  Compile
    
    ```bash
    $ cargo build --release
    ```
    
5.  After compilation, run
    
    ```bash
    $ cargo run --release -- --model assets/models/RWKV-4-World-0.4B-v1-20230529-ctx4096.st
    ```
    
6.  Open the browser and visit the WebUI [`http://127.0.0.1:3000`](http://127.0.0.1:3000)
    

## 📝Supported Arguments

*   `--model`: Model path
*   `--tokenizer`: Tokenizer path
*   `--port`: Running port

## 📙Currently Available APIs

The API service starts at port 3000, and the data input and output format follow the Openai API specification.

*   `/v1/chat/completions`
*   `/chat/completions`
*   `/v1/completions`
*   `/completions`
*   `/v1/embeddings`
*   `/embeddings`

## 📙WebUI Screenshots

![image](https://github.com/cgisky1980/ai00_rwkv_server/assets/82481660/33e8da0b-5d3f-4dfc-bf35-4a8147d099bc)

![image](https://github.com/cgisky1980/ai00_rwkv_server/assets/82481660/a24d6c72-31a0-4ff7-8a61-6eb98aae46e8)

## 📝TODO List

*   [x] Support for `text_completions` and `chat_completions`
*   [x] Support for sse push
*   [x] Add `embeddings`
*   [x] Integrate basic front-end
*   [ ] Parallel inference via `batch serve`
*   [ ] Support for `int8` quantization
*   [ ] Support for `SpQR` quantization
*   [ ] Support for `LoRA` model
*   [ ] Hot loading and switching of `LoRA` model

## 👥Join Us

We are always looking for people interested in helping us improve the project. If you are interested in any of the following, please join us!

*   💀Writing code
*   💬Providing feedback
*   🔆Proposing ideas or needs
*   🔍Testing new features
*   ✏Translating documentation
*   📣Promoting the project
*   🏅Anything else that would be helpful to us

No matter your skill level, we welcome you to join us. You can join us in the following ways:

*   Join our Discord channel
*   Join our QQ group
*   Submit issues or pull requests on GitHub
*   Leave feedback on our website

We can't wait to work with you to make this project better! We hope the project is helpful to you!


## Thank you to these awesome individuals who are insightful and outstanding for their support and selfless dedication to the project
<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/cgisky1980"><img src="https://avatars.githubusercontent.com/u/82481660?v=4?s=100" width="100px;" alt="顾真牛"/><br /><sub><b>顾真牛</b></sub></a><br /><a href="https://github.com/cgisky1980/ai00_rwkv_server/commits?author=cgisky1980" title="Documentation">📖</a> <a href="https://github.com/cgisky1980/ai00_rwkv_server/commits?author=cgisky1980" title="Code">💻</a> <a href="#content-cgisky1980" title="Content">🖋</a> <a href="#design-cgisky1980" title="Design">🎨</a> <a href="#mentoring-cgisky1980" title="Mentoring">🧑‍🏫</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://cryscan.github.io/profile"><img src="https://avatars.githubusercontent.com/u/16053640?v=4?s=100" width="100px;" alt="研究社交"/><br /><sub><b>研究社交</b></sub></a><br /><a href="https://github.com/cgisky1980/ai00_rwkv_server/commits?author=cryscan" title="Code">💻</a> <a href="#example-cryscan" title="Examples">💡</a> <a href="#ideas-cryscan" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-cryscan" title="Maintenance">🚧</a> <a href="https://github.com/cgisky1980/ai00_rwkv_server/pulls?q=is%3Apr+reviewed-by%3Acryscan" title="Reviewed Pull Requests">👀</a> <a href="#platform-cryscan" title="Packaging/porting to new platform">📦</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/josStorer"><img src="https://avatars.githubusercontent.com/u/13366013?v=4?s=100" width="100px;" alt="josc146"/><br /><sub><b>josc146</b></sub></a><br /><a href="https://github.com/cgisky1980/ai00_rwkv_server/issues?q=author%3AjosStorer" title="Bug reports">🐛</a> <a href="https://github.com/cgisky1980/ai00_rwkv_server/commits?author=josStorer" title="Code">💻</a> <a href="#ideas-josStorer" title="Ideas, Planning, & Feedback">🤔</a> <a href="#tool-josStorer" title="Tools">🔧</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/l15y"><img src="https://avatars.githubusercontent.com/u/11372524?v=4?s=100" width="100px;" alt="l15y"/><br /><sub><b>l15y</b></sub></a><br /><a href="#tool-l15y" title="Tools">🔧</a> <a href="#plugin-l15y" title="Plugin/utility libraries">🔌</a> <a href="https://github.com/cgisky1980/ai00_rwkv_server/commits?author=l15y" title="Code">💻</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->


## Stargazers over time

[![Stargazers over time](https://starchart.cc/cgisky1980/ai00_rwkv_server.svg)](https://starchart.cc/cgisky1980/ai00_rwkv_server)