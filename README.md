# Computer-Architecture-Project-4

## 프로젝트 소개
프로그램의 메모리 접근 패턴이 캐시 구조와 AMAT(Average Memory Access Time)에 어떤 영향을 미치는지 분석한 프로젝트입니다. SimpleScalar 시뮬레이터에서 block size, associativity, unified/split 구조를 단계적으로 변경하며 성능 변화를 정량적으로 비교했습니다.

## 프로젝트 개요
- 프로젝트명: Cache Performance Analysis
- 분야: Computer Architecture / Memory Hierarchy
- 실행 환경: SimpleScalar Simulator
- 실험 대상 프로그램: Bubble Sort, Random Access, go, m88ksim, swim
- 목적:
  - 각 프로그램의 메모리 접근 패턴 분석
  - 캐시 구성 변경이 Miss Rate · Penalty · AMAT에 미치는 영향 측정
  - 프로그램별 최적 Cache 구조 도출

## 주요 실험 결과 요약
- Block size 증가 시 대부분 프로그램에서 Miss Rate·AMAT이 크게 감소
- swim과 같이 spatial locality가 강한 프로그램일수록 block size 증가 효과가 큼
- go처럼 branch-heavy 패턴의 경우 unified보다 split 구조가 더 효율적
- 프로그램의 접근 패턴에 따라 최적 캐시 구조는 서로 다르게 결정됨
