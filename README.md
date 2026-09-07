# CardGame

Unity와 C#으로 제작한 카드 전략 게임 프로젝트입니다.

## 프로젝트 구조

- `Assets/Scene`  
  실제 게임에 사용되는 Unity Scene 파일(.unity)이 들어 있습니다.

- `Assets/Image`  
  카드, UI 등 게임에서 사용한 이미지 리소스가 들어 있습니다.

- `Assets/AI`  
  MCTS 기반 AI 관련 스크립트가 들어 있습니다.  
  UCB1, Hand Sampling, Selection/Expansion/Simulation/Backpropagation 로직을 확인할 수 있습니다.

- `Assets/Models`  
  머신러닝 관련 데이터 및 테스트용 더미 데이터가 들어 있습니다.

- `Assets/UI`  
  게임 UI 및 화면 동작을 처리하는 C# 스크립트가 들어 있습니다.

## 주요 기술

- Unity / C#
- MCTS 기반 AI
- UCB1
- Hand Sampling
- 게임 로직 및 UI 구현
