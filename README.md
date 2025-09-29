# Diffusion-based-Adversarial-Attack-Patch-Military-Camouflage-Pattern-
본 연구는 AI 기반 객체 탐지 기술의 발전으로 전통적인 위장무늬의 효과가 감소하는 현대 전장 환경에 대응하기 위해, 군 디지털 위장무늬와 유사한 적대적 패치 설계 방법을 제안한다. 기존 연구의 인공적 패턴과 달리, 본 연구는 diffusion 기반 생성 아키텍처를 활용하여 실제 군복과 자연스럽게 조화되는 패치를 제작하였다. YOLOv5 실험 결과, 제안된 패치는 기존 기법과 유사한 공격 성공률을 보이면서도 위장 성능 평가에서 뛰어난 은밀성을 확보하였다. 이는 AI 탐지 회피와 인간 육안 은폐를 동시에 달성하는 실용적인 군사 위장 솔루션을 제시한다.

연구자: 임서윤1 , 맹원철1 , 정성찬1 

[ ABSTRACT ]
  The advancement of AI-based object detection systems in modern warfare has significantly reduced the effectiveness of traditional camouflage patterns, even those that are difficult to identify with the human eye. In response to these changing battlefield environments, new approaches are required to minimize the risk of enemy identification. This study proposes a method for designing adversarial patches similar to military digital camouflage patterns. Existing adversarial patch research primarily employs artificial geometric patterns that are easily identifiable by human observation in actual military environments, presenting significant limitations. To address this issue, we utilized a diffusion-based patch generation architecture to create natural patches that harmonize with actual military uniforms. Experimental validation targeting YOLOv5 models demonstrated the effectiveness of degrading person detection performance. Results showed that the proposed patches achieved comparable attack success rates to existing methods while proving superior stealth against human visual identification through camouflage performance evaluation metrics. This research provides a practical military camouflage solution that simultaneously satisfies AI detection evasion and human visual concealment requirements.

Datasets
1. LoRA 학습 시 활용한 자체 제작한 군복 크롭 50장 규모
2. INRIA 904장 규모(트레인 616 테스트 288)
3. 인터넷에서 수집한 공개된 군인데이터셋 904장 규모(트레인 616 테스트 288) 실제로 활용은 하지 않았음.

코드 실행 환경 및 방법
1. 패치 제작 환경: A100-40GB
2. 패치 데이터셋 구성: INRIA VOC 구조(Train/Test의 {JPEGImages,Annotations} 또는 INRIAPerson/VOCdevkit/VOC2007/...)를 YOLO 형식으로 변환하고 640x640 letterbox 정규화, 패딩은 회색 패딩 이용
3. LoRA 학습 시 활용한 자체 제작한 군복 크롭 50장 규모 614*614로 변환하여 사용
4. 용량문제로 yolo 가중치 파일 등은 첨부하지 않았습니다.
5. stable diffusion 1.4 모델을 속도 등의 문제로 로컬로 다운받아 사용하였습니다.
6. 폴더 구조
![화면 캡처 2025-09-29 142913](https://github.com/user-attachments/assets/35efcc89-e47a-4fbb-b44f-d898f8945fb4)


문의: aod05062@gmail.com
