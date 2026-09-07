# CardGame

Unity와 C#으로 제작한 야구 전략 TCG 프로젝트입니다.

## 프로젝트 구조

- `Assets/Scenes`
  실제 게임에 사용되는 Unity Scene(.unity) 파일이 들어 있습니다.

- `Assets/Image`
  카드, 배경, 스코어보드 등 게임에서 사용되는 이미지 리소스가 들어 있습니다.

- `Assets/AI`
  MCTS 기반 AI 관련 C# 스크립트가 들어 있습니다.
  UCB1, 상대 패 샘플링, Selection / Expansion / Simulation / Backpropagation 로직을 확인할 수 있습니다.

- `Assets/Models`
  ONNX 모델 관련 데이터 파일이 포함되어 있습니다.

- `Assets/UI/Scripts`
  게임 진행, 카드 조작, 덱 구성, 스코어보드 등 UI 및 게임 로직 관련 C# 스크립트가 들어 있습니다.

- `Assets/Prefabs`
  카드와 UI 요소 등에 사용되는 Unity Prefab 파일이 들어 있습니다.

## 주요 기술

- Unity 2022.3
- C#
- MCTS 기반 게임 AI
- UCB1
- Opponent Hand Sampling
- 게임 로직 및 UI 구현
