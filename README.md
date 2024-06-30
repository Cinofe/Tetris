# Air Tetris

## 프로젝트 소개
Air Tetris는 전통적인 테트리스의 한계를 뛰어넘어, 손 모양 인식을 통해 새로운 게임 경험을 제공합니다. 기존 테트리스는 키보드 버튼을 사용하여 조작하지만, Air Tetris는 카메라를 통해 플레이어의 손 모양을 인식하여 게임을 진행합니다. 이 프로젝트는 대학 강의를 개인 프로젝트로 개발되었으며, 교내 성과 발표회에서 대상을 수상받았습니다.

## 주요 기능
- **손 모양 인식**: 키보드를 사용하지 않고, 손의 움직임만으로 블록을 조작할 수 있습니다.
- **실시간 반응**: 손 모양을 실시간으로 인식하여 게임에 반영합니다.

## 기술 상세
### 손 추적 기술
 Air Tetris는 Mediapipe와 K-NN(K-Nearest Neighbor) 알고리즘을 사용하여 손 모양을 추적합니다. 이 두 기술의 결합으로 정교하고 정확한 손 모양 인식이 가능합니다.

- **Mediapipe**: Google에서 개발한 Mediapipe는 다양한 멀티모달 머신러닝 파이프라인을 제공하며, 그 중에서도 특히 손 모양 인식에 강점을 보입니다. Mediapipe는 손의 21개 주요 관절을 실시간으로 추적하여 높은 정확도의 데이터를 제공합니다.
- **K-NN(K-Nearest Neighbor)**: K-NN 알고리즘은 손 모양 데이터를 기반으로 가장 가까운 이웃 데이터를 찾아 분류하는 데 사용됩니다. 이 알고리즘은 학습 과정이 간단하고, 실시간으로 빠르게 모양할 수 있어 손 모양 인식에 적합합니다.

### 구현 과정
1. **데이터 수집**: 손 모양 데이터를 수집하여 학습 데이터셋을 구성합니다.

      ![acd](https://github.com/Cinofe/Tetris/assets/83103532/08cc5ce1-bd70-4ab4-9c11-f6fa98080974)

3. **데이터 전처리**: 수집된 데이터셋 중 손목 부터 손 끝까지 이어지는 점들의 벡터를 계산합니다.
4. **모델 학습**: K-NN 알고리즘을 사용하여 전처리된 데이터로 모델을 학습시킵니다.
5. **실시간 추적**: 학습된 모델을 사용하여 실시간으로 손 모양을 추적하고, 이를 게임에 반영합니다.

## 프로젝트 성과
Air Tetris는 창의적인 아이디어로 주목받았으며, 교내 성과 발표회에서 대상을 수상하였습니다. 또한, 손 모양 인식 기술을 게임에 적용함으로써 사용자들에게 새로운 경험을 제공하였습니다.

## 결론
Air Tetris는 단순한 게임을 넘어, 손 모양 인식을 통해 새로운 인터페이스의 가능성을 보여줍니다. 앞으로도 이와 같은 창의적인 프로젝트를 통해 더 많은 사람들에게 즐거움을 선사할 수 있기를 기대합니다.
