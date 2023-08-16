# React test

## Section 1

### TDD(test driven development)

- "테스트를 먼저 작성하고 코드를 나중에 작성하라”
- 코드 짜기 전에 테스트케이스부터 작성 → 테스트 통과하도록 코드 작성 → 리팩토링

## Section2

### Simple App

```tsx
import { render, screen, fireEvent } from "@testing-library/react";
```

- fireEvent
    - 버튼 클릭, 폼 제출 등 가상 이벤트 트리거 시뮬레이션
- jest-dom assertions:
    - toBeEnabled() :선택한 요소가 활성화되어 있는지 확인 (예: 버튼이 클릭 가능한 상태)
    - toBeDisabled() : 선택한 요소가 비활성화되어 있는지 확인(예: 비활성화된 입력 필드)
    - toBeChecked() : 선택한 체크박스나 라디오 버튼이 체크된 상태인지 확인
- getByRole option {name: }
    - 특정 역할(role)을 가진 DOM 요소를 선택하는 메서드
    - 라벨링이나 설명을 가진 요소를 찾을 때 유용
- https://github.com/testing-library/jest-dom
- https://testing-library.com/docs/react-testing-library/intro