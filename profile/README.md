<div align="center">

# 🦊 Ofox AI

### Enterprise-grade LLM Gateway · 企业级 LLM 网关

[![Docs](https://img.shields.io/badge/Docs-blue?style=for-the-badge)](https://docs.ofox.ai)
[![Community](https://img.shields.io/badge/Community-green?style=for-the-badge)](https://github.com/ofoxai/community)
[![Status](https://img.shields.io/badge/Status-orange?style=for-the-badge)](https://status.ofox.ai)

---

### 🌐 Access OfoxAI / 访问 OfoxAI

<table>
  <tr>
    <td align="center" width="50%">
      <a href="https://ofox.ai"><img src="https://img.shields.io/badge/ofox.ai-000000?style=for-the-badge" alt="ofox.ai"/></a>
      <br/>
      <sub><b>Global</b> · 主站</sub>
    </td>
    <td align="center" width="50%">
      <a href="https://ofox.io"><img src="https://img.shields.io/badge/ofox.io-1F2328?style=for-the-badge" alt="ofox.io"/></a>
      <br/>
      <sub><b>China Mirror</b> · 中国站</sub>
    </td>
  </tr>
</table>

**English** | **中文**

</div>

<br/>

---

## 🇺🇸 English

**One unified gateway for OpenAI, Anthropic, Google Gemini, Mistral, DeepSeek, Qwen, and 100+ more models.**

- **Three native protocols** — drop-in compatible with OpenAI / Anthropic / Gemini SDKs, no client rewrites
- **Officially partnered upstreams** — direct contracts with Azure OpenAI, AWS Bedrock, Google Vertex, Anthropic, Mistral
- **Pay-as-you-go** — no subscriptions, no minimums, balances never expire
- **Enterprise-ready** — multi-member teams, role-based permissions, encrypted API key storage
- **Real-time dashboards** — usage, cost, and per-request analytics out of the box
- **Production hardened** — multi-provider failover, structured error mapping, OpenAPI-spec'd
- **Two domains, one platform** — primary `ofox.ai`, mirror `ofox.io` for resilience

### Quick Start

```bash
# Use any OpenAI-compatible SDK
export OPENAI_API_KEY="sk-ofox-..."
export OPENAI_BASE_URL="https://api.ofox.ai/v1"
```

```python
from openai import OpenAI

client = OpenAI()  # picks up the env vars above
resp = client.chat.completions.create(
    model="anthropic/claude-sonnet-4.5",   # any provider, one API
    messages=[{"role": "user", "content": "Hello!"}],
)
print(resp.choices[0].message.content)
```

Get your API key → **[app.ofox.ai](https://app.ofox.ai)** · Docs → **[docs.ofox.ai](https://docs.ofox.ai)**

<br/>

---

## 🇨🇳 中文

**企业级 LLM 网关 — 一个统一入口接入 OpenAI / Anthropic / Google Gemini / Mistral / DeepSeek / 通义千问 等 100+ 模型。**

- **三协议原生支持** — OpenAI / Anthropic / Gemini 三套官方 SDK 直接兼容，已有代码零改动
- **官方云厂商合作** — Azure / AWS / Google / Anthropic / Mistral 全部走官方授权通道
- **零订阅** — 按量付费，最低充值 $1，余额永不过期
- **多成员团队管理** — 角色权限分配，API Key 加密存储
- **实时数据看板** — 用量、费用、请求明细全链路可视化
- **双域容灾** — 主站 `ofox.ai`，镜像站 `ofox.io`，任一可用即可访问

### 快速接入

```bash
# 任何兼容 OpenAI 协议的 SDK 都可以
export OPENAI_API_KEY="sk-ofox-..."
export OPENAI_BASE_URL="https://api.ofox.ai/v1"
# 或使用镜像站: https://api.ofox.io/v1
```

```python
from openai import OpenAI

client = OpenAI()  # 自动读取上面的环境变量
resp = client.chat.completions.create(
    model="anthropic/claude-sonnet-4.5",   # 任意上游, 统一 API
    messages=[{"role": "user", "content": "你好!"}],
)
print(resp.choices[0].message.content)
```

注册领取 API Key → **[app.ofox.ai](https://app.ofox.ai)** · 开发文档 → **[docs.ofox.ai](https://docs.ofox.ai)**

<br/>

---

## 🔌 SDK 兼容矩阵 / SDK Compatibility

| Protocol | Endpoint (Primary) | Endpoint (Mirror) | One-line change |
|---|---|---|---|
| **OpenAI** | `https://api.ofox.ai/v1` | `https://api.ofox.io/v1` | `base_url=` |
| **Anthropic** | `https://api.ofox.ai/anthropic` | `https://api.ofox.io/anthropic` | `base_url=` |
| **Gemini** | `https://api.ofox.ai/gemini` | `https://api.ofox.io/gemini` | `base_url=` |

Works with: `openai`, `anthropic`, `@google/generative-ai`, `langchain`, `llamaindex`, `vercel/ai`, `cursor`, `cherry-studio`, `claude-code`, `gemini-cli`, `openclaw`, and anything that respects `OPENAI_BASE_URL`.

<br/>

---

## 🏢 Why teams choose OfoxAI / 团队为什么选择 OfoxAI

<table>
  <tr>
    <td align="center" width="33%">
      <h4>🤝 Official upstream partners</h4>
      <sub><b>官方云厂商合作</b></sub><br/>
      <sub>Azure · AWS Bedrock · Google Vertex · Anthropic · Mistral — direct contracts, no resellers</sub>
    </td>
    <td align="center" width="33%">
      <h4>👥 Team & permissions</h4>
      <sub><b>多成员团队管理</b></sub><br/>
      <sub>Role-based access, encrypted API key storage, audit trails</sub>
    </td>
    <td align="center" width="33%">
      <h4>📊 Real-time analytics</h4>
      <sub><b>实时数据看板</b></sub><br/>
      <sub>Per-token cost, latency, request history — all in your dashboard</sub>
    </td>
  </tr>
</table>

<br/>

---

## 🧭 Resources

<table>
  <tr>
    <td align="center" width="25%">
      <a href="https://docs.ofox.ai"><b>📖 Docs</b></a><br/>
      <sub>API reference · SDK guides · Integrations</sub>
    </td>
    <td align="center" width="25%">
      <a href="https://ofox.ai/pricing"><b>💰 Pricing</b></a><br/>
      <sub>Per-token billing · Volume discounts</sub>
    </td>
    <td align="center" width="25%">
      <a href="https://status.ofox.ai"><b>📊 Status</b></a><br/>
      <sub>Real-time uptime · Provider health</sub>
    </td>
    <td align="center" width="25%">
      <a href="https://github.com/ofoxai/community"><b>💬 Community</b></a><br/>
      <sub>Discussions · Bug reports · Feedback</sub>
    </td>
  </tr>
</table>

<br/>

---

<div align="center">

**Singapore 🇸🇬** · [@ofox_ai](https://twitter.com/ofox_ai) · [hi@ofox.ai](mailto:hi@ofox.ai)

<sub>🦊 Built for developers and teams who ship.</sub>

<br/><br/>

<sub>© NICE TALK PTE. LTD. · Singapore · UEN registered</sub>

</div>
