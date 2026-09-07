# CardGame - 야구 전략 TCG 「봉황대기」

Unity와 C#으로 제작한 야구 전략 TCG 졸업작품입니다.  
야구의 공격·수비 요소와 카드 전략을 결합했으며, 플레이어가 다양한 덱과 전략을 활용해 AI와 대결할 수 있도록 구현했습니다.

## 프로젝트 개요

- 개발 환경: Unity 2022.3.62f3
- 개발 언어: C#
- 프로젝트 형태: 졸업작품 / 팀 프로젝트
- 주요 담당: 게임 코어 로직, AI 시스템, 덱 시스템, UI 및 게임 진행 기능 구현

## 주요 구현 내용

### 1. 게임 시스템
- 카드 Drag & Drop 방식의 카드 사용 기능 구현
- 공격·수비 및 득점 처리 로직 구현
- End Turn UI 위치 및 게임 진행 흐름 개선
- 덱 구성 및 관리 시스템 구현
- 카드별 특수 능력 구현
- 게임 로그 시스템 개선

### 2. AI 시스템
- MCTS(Monte Carlo Tree Search) 기반 AI 의사결정 시스템 구현
- Selection / Expansion / Simulation / Backpropagation 구조 구현
- UCB1 공식을 활용한 탐색 노드 선택
- 상대의 비공개 패를 고려하기 위한 Hand Sampling 적용
- 현재 게임 상태를 기반으로 AI가 행동을 선택하도록 GameState 구조 활용
- Coroutine을 사용해 AI 행동에 지연 시간을 적용하여 자연스러운 게임 진행 구현

### 3. UI / UX
- 카드별 UI 구현
- 스코어보드 구현
- 타이틀 Scene 제작
- 동전 던지기 기능 및 연출 구현
- 동전 던지기 진행 중 다른 카드와 UI를 숨기도록 화면 처리
- 튜토리얼 Scene 및 진행 로직 구현
- 게임 진행 상황을 확인할 수 있도록 로그 UI 개선

## 프로젝트 구조

### Assets/Scenes
실제 게임에서 사용되는 Unity Scene(.unity) 파일들이 들어 있습니다.

### Assets/Image
카드, 배경, 스코어보드 등 게임에서 사용되는 이미지 리소스가 들어 있습니다.

### Assets/AI
MCTS 기반 AI 관련 C# 스크립트가 들어 있습니다.

주요 구현 내용:
- MCTS 탐색
- UCB1
- Hand Sampling
- Selection / Expansion / Simulation / Backpropagation
- GameState 기반 게임 상태 처리

### Assets/UI/Scripts
게임 진행, 카드 조작, 덱 구성, 스코어보드 등 UI 및 게임 로직 관련 C# 스크립트가 들어 있습니다.

### Assets/Models
ONNX 모델 관련 데이터 파일이 포함되어 있습니다.

### Assets/Prefabs
카드 및 UI 요소 등에 사용되는 Unity Prefab 파일들이 들어 있습니다.

## 주요 기술

- Unity
- C#
- MCTS
- UCB1
- Hand Sampling
- Coroutine
- Unity UI
- GameState 기반 게임 상태 관리
- Drag & Drop
- Deck System
