# 읽어보기

- 원문 저장소: `langchain-ai/langchain`
- 미러 저장소: `martinlee-git/langchain`
- 원문 문서: https://github.com/langchain-ai/langchain/blob/master/libs/model-profiles/README.md
- 미러 경로: `libs/model-profiles/README.md`

## 한글 요약

🦜🪪 langchain 모델 프로필 [!경고] 이 패키지는 현재 개발 중이며 API는 변경될 수 있습니다. LangChain 통합 패키지의 모델 프로필 데이터를 업데이트하기 위한 CLI 도구입니다. 빠른 설치 🤔 이게 뭔가요? langchain 모델 프로필은 LangChain 통합 패키지에서 사용하기 위해 models.dev에서 모델 기능 데이터를 가져오고 업데이트하는 CLI 도구입니다. LangChain 채팅 모델은 컨텍스트 창 크기, 지원되는 양식, 도구 호출, 구조화된 출력 등과 같은 모델 기능에 대한 프로그래밍 방식의 액세스를 제공하는 .profile 필드를 노출합니다. 이 CLI 도구는 관리자가 해당 데이터를 최신 상태로 유지하는 데 도움이 됩니다. 데이터 소스 이 패키지는 모델 기능 데이터를 제공하는 오픈 소스 이니셔티브인 models.dev 프로젝트의 뛰어난 작업을 기반으로 구축되었습니다. LangChain 모델 프로필은 몇 가지 추가 필드를 사용하여 models.dev의 데이터를 보강합니다. 우리는 이를 업스트림 프로젝트가 발전함에 따라 계속해서 조정할 계획입니다. 📖 문서 전체 문서를 보려면 API 참조를 확인하세요.

## 핵심 발췌

. LangChain 사용에 대한 개념적 가이드, 튜토리얼 및 예제는 LangChain Docs를 참조하세요. Chat LangChain을 사용하여 문서와 채팅할 수도 있습니다. 특정 공급자에 대한 사용 업데이트 모델 프로필 데이터: 이는 models.dev에서 최신 모델 데이터를 다운로드하고 이를 프로필 Augmentations.toml에 정의된 모든 기능 보강과 병합한 후 프로필.py 파일을 생성합니다.

## 원문 내용

# 🦜🪪 langchain-model-profiles

[![PyPI - Version](https://img.shields.io/pypi/v/langchain-model-profiles?label=%20)](https://pypi.org/project/langchain-model-profiles/#history)
[![PyPI - License](https://img.shields.io/pypi/l/langchain-model-profiles)](https://opensource.org/licenses/MIT)
[![PyPI - Downloads](https://img.shields.io/pepy/dt/langchain-model-profiles)](https://pypistats.org/packages/langchain-model-profiles)
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchain_oss.svg?style=social&label=Follow%20%40LangChain)](https://x.com/langchain_oss)

> [!WARNING]
> This package is currently in development and the API is subject to change.

CLI tool for updating model profile data in LangChain integration packages.

## Quick Install

```bash
pip install langchain-model-profiles
```

## 🤔 What is this?

`langchain-model-profiles` is a CLI tool for fetching and updating model capability data from [models.dev](https://github.com/sst/models.dev) for use in LangChain integration packages.

LangChain chat models expose a `.profile` field that provides programmatic access to model capabilities such as context window sizes, supported modalities, tool calling, structured output, and more. This CLI tool helps maintainers keep that data up-to-date.

## Data sources

This package is built on top of the excellent work by the [models.dev](https://github.com/sst/models.dev) project, an open source initiative that provides model capability data.

LangChain model profiles augment the data from models.dev with some additional fields. We intend to keep this aligned with the upstream project as it evolves.

## 📖 Documentation

For full documentation, see the [API reference](https://reference.langchain.com/python/langchain_model_profiles/). For conceptual guides, tutorials, and examples on using LangChain, see the [LangChain Docs](https://docs.langchain.com/oss/python/langchain/overview). You can also chat with the docs using [Chat LangChain](https://chat.langchain.com).

## Usage

Update model profile data for a specific provider:

```bash
langchain-profiles refresh --provider anthropic --data-dir ./langchain_anthropic/data
```

This downloads the latest model data from models.dev, merges it with any augmentations defined in `profile_augmentations.toml`, and generates a `profiles.py` file.