# 읽어보기

- 원문 저장소: `langchain-ai/langchain`
- 미러 저장소: `martinlee-git/langchain`
- 원문 문서: https://github.com/langchain-ai/langchain/blob/master/libs/partners/huggingface/README.md
- 미러 경로: `libs/partners/huggingface/README.md`

## 한글 요약

langchainhuggingface JS/TS 버전을 찾고 계십니까? LangChain.js를 확인해 보세요. 빠른 설치 참고: 기본 설치에는 문장 변환기 또는 변환기가 포함되지 않습니다. 로컬 추론을 위해 HuggingFaceEmbeddings 또는 HuggingFacePipeline을 사용하려는 경우 문장 변환기 =5.2.0 및 변환기 =5.0.0을 포함하는 [전체] 추가 항목을 설치하십시오: langchain 커뮤니티에서 마이그레이션하시겠습니까? langchain 커뮤니티에서는 문장 변환기 =2.2.0을 허용했지만 langchainhuggingface[full]에는 =5.2.0이 필요합니다. 프로젝트에 이전 버전이 고정되어 있으면 업그레이드하세요. 🤔 이게 뭐죠? 이 패키지에는 Hugging Face 관련 클래스에 대한 LangChain 통합이 포함되어 있습니다. 📖 문서 전체 문서를 보려면 API 참조를 확인하세요. 이러한 클래스 사용에 대한 개념적 가이드, 튜토리얼 및 예제는 LangChain Docs를 참조하세요. 📕 릴리스 및 버전 관리 릴리스 및 버전 관리 정책을 참조하세요. 💁 기여 빠르게 발전하는 분야의 오픈 소스 프로젝트로서 우리는 기여에 대해 매우 개방적입니다.

## 핵심 발췌

r 새로운 기능, 향상된 인프라 또는 더 나은 문서의 형태일 수 있습니다. 기여 방법에 대한 자세한 내용은 기여 가이드를 참조하세요. 리소스 LangChain Academy — LangChain 팀에서 만든 LangChain 라이브러리 및 제품에 대한 포괄적인 무료 코스, 행동 강령 — 커뮤니티 지침 및 표준

## 원문 내용

# langchain-huggingface

[![PyPI - Version](https://img.shields.io/pypi/v/langchain-huggingface?label=%20)](https://pypi.org/project/langchain-huggingface/#history)
[![PyPI - License](https://img.shields.io/pypi/l/langchain-huggingface)](https://opensource.org/licenses/MIT)
[![PyPI - Downloads](https://img.shields.io/pepy/dt/langchain-huggingface)](https://pypistats.org/packages/langchain-huggingface)
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchain_oss.svg?style=social&label=Follow%20%40LangChain)](https://x.com/langchain_oss)

Looking for the JS/TS version? Check out [LangChain.js](https://github.com/langchain-ai/langchainjs).

## Quick Install

```bash
uv add langchain-huggingface
```

> **Note:** The base install does not include `sentence-transformers` or `transformers`.
> If you plan to use `HuggingFaceEmbeddings` or `HuggingFacePipeline` for **local inference**,
> install the `[full]` extra which includes `sentence-transformers>=5.2.0` and `transformers>=5.0.0`:
>
> ```bash
> uv add "langchain-huggingface[full]"
> ```
>
> **Migrating from `langchain-community`?** Note that `langchain-community` accepted
> `sentence-transformers>=2.2.0`, but `langchain-huggingface[full]` requires `>=5.2.0`.
> If your project pins an older version, upgrade it:
>
> ```bash
> uv add "sentence-transformers>=5.2.0"
> ```

## 🤔 What is this?

This package contains the LangChain integrations for Hugging Face related classes.

## 📖 Documentation

For full documentation, see the [API reference](https://reference.langchain.com/python/integrations/langchain_huggingface/). For conceptual guides, tutorials, and examples on using these classes, see the [LangChain Docs](https://docs.langchain.com/oss/python/integrations/providers/huggingface).

## 📕 Releases & Versioning

See our [Releases](https://docs.langchain.com/oss/python/release-policy) and [Versioning](https://docs.langchain.com/oss/python/versioning) policies.

## 💁 Contributing

As an open-source project in a rapidly developing field, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.

For detailed information on how to contribute, see the [Contributing Guide](https://docs.langchain.com/oss/python/contributing/overview).

## Resources

- [LangChain Academy](https://academy.langchain.com/) — comprehensive, free courses on LangChain libraries and products, made by the LangChain team
- [Code of Conduct](https://github.com/langchain-ai/langchain/?tab=coc-ov-file) — community guidelines and standards