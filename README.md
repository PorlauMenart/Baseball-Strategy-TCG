# 봉황대기 - Baseball Strategy TCG

Unity와 C#으로 제작한 야구 전략 TCG 졸업작품입니다.  
야구의 공격·수비 규칙과 카드 전략 요소를 결합했으며,
플레이어가 직접 덱을 구성해 AI와 대결할 수 있도록 구현했습니다.

## 개발 환경

- Unity 2022.3.62f3
- C#
- MCTS (Monte Carlo Tree Search)
- UCB1
- Opponent Hand Sampling
- Coroutine
- Unity UI

## 담당 역할

- 게임 코어 로직 구현
- MCTS 기반 AI 의사결정 시스템 구현
- 상대 패 Hand Sampling 및 UCB1 적용
- 덱 구성 및 관리 시스템 구현
- 카드 Drag & Drop 구현
- 게임 UI 및 튜토리얼 구현
- 게임 로그 및 진행 흐름 개선

## 주요 구현

### Game System
- Drag & Drop 방식의 카드 사용
- 공격·수비 및 득점 처리
- 커스텀 덱 구성 시스템
- 카드별 공격·수비 및 특수 효과
- 게임 로그 및 이닝별 스코어보드

### AI System
- MCTS 기반 AI 의사결정 로직
- Selection / Expansion / Simulation / Backpropagation 구현
- UCB1 기반 탐색 노드 선택
- 상대의 비공개 패를 고려한 Hand Sampling
- GameState를 활용한 게임 규칙과 AI 시뮬레이션 연동

### UI / UX
- 카드 Drag & Drop 및 Drop Zone
- 선공·후공 결정을 위한 동전 던지기
- 동전 던지기 중 다른 UI를 숨기는 화면 처리
- Coroutine을 활용한 AI 행동 지연
- 스코어보드 및 게임 메뉴
- 튜토리얼 Scene 및 진행 로직

## 프로젝트 구조

- `Assets/Scenes`
  - 실제 게임에서 사용되는 Unity Scene

- `Assets/AI`
  - MCTS, UCB1, Hand Sampling 및 GameState 관련 코드

- `Assets/UI/Scripts`
  - 카드 조작, 덱 구성, 스코어보드, 튜토리얼 및 게임 진행 코드

- `Assets/Image`
  - 카드, 배경, UI 이미지 리소스

- `Assets/Prefabs`
  - 카드 및 UI Prefab

- `Assets/Models`
  - ONNX 모델 관련 데이터

## 주요 코드

- AI 탐색 로직  
  `Assets/AI/MCTSAgent.cs`

- MCTS 노드  
  `Assets/AI/MCTSNode.cs`

- 게임 상태  
  `Assets/AI/GameState.cs`

- 메인 게임 진행  
  `Assets/UI/Scripts/SingleLaneGame.cs`

- 카드 Drag & Drop  
  `Assets/UI/Scripts/CardDragHandler.cs`

- 덱 구성  
  `Assets/UI/Scripts/DeckBuildManager.cs`

- 튜토리얼  
  `Assets/UI/Scripts/TutorialManager.cs`

## 실행 방법

1. Unity 2022.3.x에서 프로젝트를 엽니다.
2. `Assets/Scenes/GameMenu.unity` 또는 `SingleLane.unity`를 엽니다.
3. Unity Editor에서 Play 버튼을 눌러 실행합니다.
