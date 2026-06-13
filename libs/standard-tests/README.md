# 읽어보기

- 원문 저장소: `langchain-ai/langchain`
- 미러 저장소: `martinlee-git/langchain`
- 원문 문서: https://github.com/langchain-ai/langchain/blob/master/libs/standard-tests/README.md
- 미러 경로: `libs/standard-tests/README.md`

## 한글 요약

🦜️🔗 langchain 테스트 JS/TS 버전을 찾고 계십니까? LangChain.js를 확인해 보세요. 빠른 설치 🤔 이게 뭔가요? 이것은 LangChain 통합을 위한 테스트 라이브러리입니다. 여기에는 표준 테스트 세트에 대한 기본 클래스가 포함되어 있습니다. 📖 문서 전체 문서를 보려면 API 참조를 확인하세요. 📕 릴리스 및 버전 관리 릴리스 및 버전 관리 정책을 참조하세요. 새 테스트를 게시할 때 CI가 손상되는 것을 방지하려면 버전을 특정 버전에 고정하는 것이 좋습니다. 최신 테스트를 받을 수 있도록 주기적으로 최신 버전으로 업그레이드하는 것이 좋습니다. 버전을 고정하지 않으면 항상 최신 테스트를 받을 수 있지만, 통합이 통과하지 못한 테스트를 도입하면 CI가 손상될 수도 있습니다. 💁 기여 빠르게 발전하는 분야의 오픈 소스 프로젝트로서 우리는 새로운 기능, 개선된 인프라, 더 나은 문서 등의 형태로 기여하는 데 매우 열려 있습니다. 기여 방법에 대한 자세한 내용은 기여하기를 참조하세요.

## 핵심 발췌

가이드. 사용법 통합 패키지(예: 채팅 모델용)에 표준 테스트를 추가하려면 다음을 생성해야 합니다. 1. ChatModelUnitTests에서 상속되는 단위 테스트 클래스 2. ChatModelIntegrationTests에서 상속되는 통합 테스트 클래스 테스트/단위 테스트/test Standard.py: 테스트/통합 테스트/테스트 표준.py: 참조 테스트 클래스에서 다음 픽스처를 구성할 수 있습니다. 필수로 표시되지 않은 사항은 선택 사항입니다. 채팅 모델 클래스(필수): 테스트할 채팅 모델의 클래스 채팅 모델 매개변수: 채팅 모델 생성자에 전달할 키워드 인수 채팅 모델에는 도구 호출이 있습니다. 채팅 모델이 도구를 호출할 수 있는지 여부입니다. 기본적으로 이는 hasattr(채팅 모델 클래스, '바인드 도구)로 설정됩니다. 채팅 모델에는 구조화된 출력이 있습니다. 채팅 모델이 구조화된 출력을 할 수 있는지 여부입니다. By d

## 원문 내용

# 🦜️🔗 langchain-tests

[![PyPI - Version](https://img.shields.io/pypi/v/langchain-tests?label=%20)](https://pypi.org/project/langchain-tests/#history)
[![PyPI - License](https://img.shields.io/pypi/l/langchain-tests)](https://opensource.org/licenses/MIT)
[![PyPI - Downloads](https://img.shields.io/pepy/dt/langchain-tests)](https://pypistats.org/packages/langchain-tests)
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchain_oss.svg?style=social&label=Follow%20%40LangChain)](https://x.com/langchain_oss)

Looking for the JS/TS version? Check out [LangChain.js](https://github.com/langchain-ai/langchainjs).

## Quick Install

```bash
uv add langchain-tests
```

## 🤔 What is this?

This is a testing library for LangChain integrations. It contains the base classes for a standard set of tests.

## 📖 Documentation

For full documentation, see the [API reference](https://reference.langchain.com/python/langchain_tests/).

## 📕 Releases & Versioning

See our [Releases](https://docs.langchain.com/oss/python/release-policy) and [Versioning](https://docs.langchain.com/oss/python/versioning) policies.

We encourage pinning your version to a specific version in order to avoid breaking your CI when we publish new tests. We recommend upgrading to the latest version periodically to make sure you have the latest tests.

Not pinning your version will ensure you always have the latest tests, but it may also break your CI if we introduce tests that your integration doesn't pass.

## 💁 Contributing

As an open-source project in a rapidly developing field, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.

For detailed information on how to contribute, see the [Contributing Guide](https://docs.langchain.com/oss/python/contributing/overview).

## Usage

To add standard tests to an integration package (e.g., for a chat model), you need to create

1. A unit test class that inherits from `ChatModelUnitTests`
2. An integration test class that inherits from `ChatModelIntegrationTests`

`tests/unit_tests/test_standard.py`:

```python
"""Standard LangChain interface tests"""

from typing import Type

import pytest
from langchain_core.language_models import BaseChatModel
from langchain_tests.unit_tests import ChatModelUnitTests

from langchain_parrot_chain import ChatParrotChain


class TestParrotChainStandard(ChatModelUnitTests):
    @pytest.fixture
    def chat_model_class(self) -> Type[BaseChatModel]:
        return ChatParrotChain
```

`tests/integration_tests/test_standard.py`:

```python
"""Standard LangChain interface tests"""

from typing import Type

import pytest
from langchain_core.language_models import BaseChatModel
from langchain_tests.integration_tests import ChatModelIntegrationTests

from langchain_parrot_chain import ChatParrotChain


class TestParrotChainStandard(ChatModelIntegrationTests):
    @pytest.fixture
    def chat_model_class(self) -> Type[BaseChatModel]:
        return ChatParrotChain
```

## Reference

The following fixtures are configurable in the test classes. Anything not marked
as required is optional.

- `chat_model_class` (required): The class of the chat model to be tested
- `chat_model_params`: The keyword arguments to pass to the chat model constructor
- `chat_model_has_tool_calling`: Whether the chat model can call tools. By default, this is set to `hasattr(chat_model_class, 'bind_tools)`
- `chat_model_has_structured_output`: Whether the chat model can structured output. By default, this is set to `hasattr(chat_model_class, 'with_structured_output')`