# 읽어보기

- 원문 저장소: `langchain-ai/langchain`
- 미러 저장소: `martinlee-git/langchain`
- 원문 문서: https://github.com/langchain-ai/langchain/blob/master/libs/core/README.md
- 미러 경로: `libs/core/README.md`

## 한글 요약

🦜🍎️ LangChain Core JS/TS 버전을 찾고 계십니까? LangChain.js를 확인해 보세요. LangChain 앱을 더 빠르게 프로덕션에 출시하려면 LangSmith를 확인하세요. LangSmith는 LLM 애플리케이션을 구축, 테스트 및 모니터링하기 위한 통합 개발자 플랫폼입니다. 빠른 설치 🤔 이게 뭔가요? LangChain Core에는 LangChain 생태계를 강화하는 기본 추상화가 포함되어 있습니다. 이러한 추상화는 가능한 한 모듈화되고 단순하게 설계되었습니다. 이러한 추상화의 이점은 모든 공급자가 필요한 인터페이스를 구현한 다음 LangChain 생태계의 나머지 부분에서 쉽게 사용할 수 있다는 것입니다. ⛰️ 왜 LangChain Core 위에 구축해야 할까요? LangChain 생태계는 Langchain 코어 위에 구축됩니다. 몇 가지 이점은 다음과 같습니다. 모듈성: 우리는 특정 모델 제공자에 묶이지 않고 서로 독립적인 추상화를 중심으로 Core를 설계했습니다. 안정성: 우리는 안정적인 버전 관리 체계를 위해 최선을 다하고 있으며, 주요 변경 사항이 있을 경우 사전 공지 및 버전 변경을 통해 알려드릴 것입니다. 전투

## 핵심 발췌

테스트됨 : 핵심 구성 요소는 LLM 생태계에서 가장 큰 설치 기반을 보유하고 있으며 많은 회사에서 생산에 사용됩니다. 📖 문서 전체 문서를 보려면 API 참조를 확인하세요. LangChain 사용에 대한 개념적 가이드, 튜토리얼 및 예제는 LangChain Docs를 참조하세요. Chat LangChain을 사용하여 문서와 채팅할 수도 있습니다. 📕 릴리스 및 버전 관리 릴리스 및 버전 관리 정책을 참조하세요. 💁 기여 빠르게 발전하는 분야의 오픈 소스 프로젝트로서 우리는 새로운 기능, 개선된 인프라, 더 나은 문서 등의 형태로 기여하는 데 매우 열려 있습니다. 기여 방법에 대한 자세한 내용은 기여 가이드를 참조하세요. 리소스 LangChain Academy — LangChain te에서 제작한 LangChain 라이브러리 및 제품에 대한 포괄적인 무료 강좌입니다.

## 원문 내용

# 🦜🍎️ LangChain Core

[![PyPI - Version](https://img.shields.io/pypi/v/langchain-core?label=%20)](https://pypi.org/project/langchain-core/#history)
[![PyPI - License](https://img.shields.io/pypi/l/langchain-core)](https://opensource.org/licenses/MIT)
[![PyPI - Downloads](https://img.shields.io/pepy/dt/langchain-core)](https://pypistats.org/packages/langchain-core)
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchain_oss.svg?style=social&label=Follow%20%40LangChain)](https://x.com/langchain_oss)

Looking for the JS/TS version? Check out [LangChain.js](https://github.com/langchain-ai/langchainjs).

To help you ship LangChain apps to production faster, check out [LangSmith](https://www.langchain.com/langsmith).
[LangSmith](https://www.langchain.com/langsmith) is a unified developer platform for building, testing, and monitoring LLM applications.

## Quick Install

```bash
uv add langchain-core
```

## 🤔 What is this?

LangChain Core contains the base abstractions that power the LangChain ecosystem.

These abstractions are designed to be as modular and simple as possible.

The benefit of having these abstractions is that any provider can implement the required interface and then easily be used in the rest of the LangChain ecosystem.

## ⛰️ Why build on top of LangChain Core?

The LangChain ecosystem is built on top of `langchain-core`. Some of the benefits:

- **Modularity**: We've designed Core around abstractions that are independent of each other, and not tied to any specific model provider.
- **Stability**: We are committed to a stable versioning scheme, and will communicate any breaking changes with advance notice and version bumps.
- **Battle-tested**: Core components have the largest install base in the LLM ecosystem, and are used in production by many companies.

## 📖 Documentation

For full documentation, see the [API reference](https://reference.langchain.com/python/langchain_core/). For conceptual guides, tutorials, and examples on using LangChain, see the [LangChain Docs](https://docs.langchain.com/oss/python/langchain/overview). You can also chat with the docs using [Chat LangChain](https://chat.langchain.com).

## 📕 Releases & Versioning

See our [Releases](https://docs.langchain.com/oss/python/release-policy) and [Versioning](https://docs.langchain.com/oss/python/versioning) policies.

## 💁 Contributing

As an open-source project in a rapidly developing field, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.

For detailed information on how to contribute, see the [Contributing Guide](https://docs.langchain.com/oss/python/contributing/overview).

## Resources

- [LangChain Academy](https://academy.langchain.com/) — comprehensive, free courses on LangChain libraries and products, made by the LangChain team
- [Code of Conduct](https://github.com/langchain-ai/langchain/?tab=coc-ov-file) — community guidelines and standards