# 읽어보기

- 원문 저장소: `langchain-ai/langchain`
- 미러 저장소: `martinlee-git/langchain`
- 원문 문서: https://github.com/langchain-ai/langchain/blob/master/README.md
- 미러 경로: `README.md`

## 한글 요약

<div align="center" <a href="https://docs.langchain.com/oss/python/langchain/overview" <picture <source media="(색 구성표 선호: 어두운)" srcset=".github/images/logo dark.svg" <source media="(색 구성표 선호: 밝은)" srcset=".github/images/logo light.svg" <img alt="LangChain 로고" src=".github/images/logo dark.svg" width="50%" </picture </a </div <div align="center" <h3 에이전트 엔지니어링 플랫폼.</h3 </div <div align="center" <a href="https://opensource.org/licenses/MIT" target=" 공백" <img src="https://img.shields.io/pypi/l/langchain" alt="PyPI 라이센스" </a <a href="https://pypistats.org/packages/langchain" target=" 공백" <img src="https://img.shields.io/pepy/dt/langchain" alt="PyPI 다운로드" </a <a href="https://pypi.org/project/langchain/#history" target=" 공백" <img src="https://img.shields.io/pypi/v/langchain?label=%20" alt="버전" </a <a href="https://x.com/langchain oss" target=" 공백" <img src="https://img.shields.io/twitter/url/https/twitter.com/langchain o

## 핵심 발췌

ss.svg?style=social&label=Follow%20%40LangChain" alt="Twitter / X" </a </div <br LangChain은 에이전트 및 LLM 기반 애플리케이션 구축을 위한 프레임워크입니다. 이는 상호 운용 가능한 구성 요소와 타사 통합을 함께 연결하여 AI 애플리케이션 개발을 단순화하는 동시에 기본 기술이 발전함에 따라 미래 보장 결정을 내리는 데 도움이 됩니다. [!팁] 이제 막 시작하시나요? Deep Agents를 확인해 보세요. 계획, 하위 에이전트, 파일 시스템 사용 등과 같은 일반적인 사용 패턴에 대한 기능이 내장된 에이전트용 LangChain 빠른 시작 고급 사용자 정의 또는 에이전트 오케스트레이션을 찾고 있다면 제어 가능한 에이전트 워크플로 구축을 위한 프레임워크인 LangGraph를 확인하세요. 동등한 JS/TS 라이브러리는 LangChain.js를 확인하세요.

## 원문 내용

<div align="center">
  <a href="https://docs.langchain.com/oss/python/langchain/overview">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset=".github/images/logo-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset=".github/images/logo-light.svg">
      <img alt="LangChain Logo" src=".github/images/logo-dark.svg" width="50%">
    </picture>
  </a>
</div>

<div align="center">
  <h3>The agent engineering platform.</h3>
</div>

<div align="center">
  <a href="https://opensource.org/licenses/MIT" target="_blank"><img src="https://img.shields.io/pypi/l/langchain" alt="PyPI - License"></a>
  <a href="https://pypistats.org/packages/langchain" target="_blank"><img src="https://img.shields.io/pepy/dt/langchain" alt="PyPI - Downloads"></a>
  <a href="https://pypi.org/project/langchain/#history" target="_blank"><img src="https://img.shields.io/pypi/v/langchain?label=%20" alt="Version"></a>
  <a href="https://x.com/langchain_oss" target="_blank"><img src="https://img.shields.io/twitter/url/https/twitter.com/langchain_oss.svg?style=social&label=Follow%20%40LangChain" alt="Twitter / X"></a>
</div>

<br>

LangChain is a framework for building agents and LLM-powered applications. It helps you chain together interoperable components and third-party integrations to simplify AI application development — all while future-proofing decisions as the underlying technology evolves.

> [!TIP]
> Just getting started? Check out **[Deep Agents](http://docs.langchain.com/oss/python/deepagents/)** — a higher-level package built on LangChain for agents that have built-in capabilites for common usage patterns such as planning, subagents, file system usage, and more.

## Quickstart

```bash
uv add langchain
```

```python
from langchain.chat_models import init_chat_model

model = init_chat_model("openai:gpt-5.5")
result = model.invoke("Hello, world!")
```

If you're looking for more advanced customization or agent orchestration, check out [LangGraph](https://github.com/langchain-ai/langgraph), our framework for building controllable agent workflows.

For an equivalent JS/TS library, check out [LangChain.js](https://github.com/langchain-ai/langchainjs).

> [!TIP]
> For developing, debugging, and deploying AI agents and LLM applications, see [LangSmith](https://docs.langchain.com/langsmith/home).

## LangChain ecosystem

While the LangChain framework can be used standalone, it also integrates seamlessly with any LangChain product, giving developers a full suite of tools when building LLM applications.

- **[Deep Agents](http://docs.langchain.com/oss/python/deepagents/)** — Build agents that can plan, use subagents, and leverage file systems for complex tasks
- **[LangGraph](https://docs.langchain.com/oss/python/langgraph/overview)** — Build agents that can reliably handle complex tasks with our low-level agent orchestration framework
- **[Integrations](https://docs.langchain.com/oss/python/integrations/providers/overview)** — Chat & embedding models, tools & toolkits, and more
- **[LangSmith](https://www.langchain.com/langsmith)** — Agent evals, observability, and debugging for LLM apps
- **[LangSmith Deployment](https://docs.langchain.com/langsmith/deployments)** — Deploy and scale agents with a purpose-built platform for long-running, stateful workflows

## Why use LangChain?

LangChain helps developers build applications powered by LLMs through a standard interface for models, embeddings, vector stores, and more.

- **Real-time data augmentation** — Easily connect LLMs to diverse data sources and external/internal systems, drawing from LangChain's vast library of integrations with model providers, tools, vector stores, retrievers, and more
- **Model interoperability** — Swap models in and out as your engineering team experiments to find the best choice for your application's needs. As the industry frontier evolves, adapt quickly — LangChain's abstractions keep you moving without losing momentum
- **Rapid prototyping** — Quickly build and iterate on LLM applications with LangChain's modular, component-based architecture. Test different approaches and workflows without rebuilding from scratch, accelerating your development cycle
- **Production-ready features** — Deploy reliable applications with built-in support for monitoring, evaluation, and debugging through integrations like LangSmith. Scale with confidence using battle-tested patterns and best practices
- **Vibrant community and ecosystem** — Leverage a rich ecosystem of integrations, templates, and community-contributed components. Benefit from continuous improvements and stay up-to-date with the latest AI developments through an active open-source community
- **Flexible abstraction layers** — Work at the level of abstraction that suits your needs — from high-level chains for quick starts to low-level components for fine-grained control. LangChain grows with your application's complexity

---

## Resources

- [Documentation](https://docs.langchain.com/oss/python/langchain/overview) — conceptual overviews and guides
- [LangChain ecosystem overview](https://docs.langchain.com/oss/python/concepts/products) — how LangChain, LangGraph, and Deep Agents fit together
- [API reference](https://reference.langchain.com/python) — complete reference for all public classes, functions, and types
- [Discussions](https://forum.langchain.com/c/oss-product-help-lc-and-lg/langchain/14) — community forum for technical questions, ideas, and feedback
- [LangChain Academy](https://academy.langchain.com/) — comprehensive, free courses on LangChain libraries and products, made by the LangChain team
- [Contributing Guide](https://docs.langchain.com/oss/python/contributing/overview) — how to contribute and find good first issues
- [Code of Conduct](https://github.com/langchain-ai/langchain/?tab=coc-ov-file) — community guidelines and standards