# Northeast Asian Age & Gender Classifier
Classifying by age and gender using a dataset of Northeast Asian face photos

## Summary of Project and Team
- Microsoft AI School Team 2 Project
- Schedule : 
    - Processing : 2023.1.13 ~ 1.16
    - A result briefing session : 2023.1.18 | Presentation : [presentation.pdf](/presentation.pdf)
- Member of Project   
    Team Leader : @yeoiksu | https://github.com/yeoiksu  
    Team Member : @TaeYounKwon | https://github.com/TaeYounKwon  
    Team Member : @ssyjgs1 | https://github.com/ssyjgs1  
    Team Member : @Byunggu-Son | https://github.com/Byunggu-Son  
    Team Member : @yuyeon | https://github.com/yuyeon-choi  
- Project Environment and Technical Stacks
    - Stacks : Python, PyTorch, Anaconda Environment, etc...
    - Environments : Processing Model on Microsoft Azure Data Science Virtual Machine

## Introduction  
본 프로젝트는 동북아시아 사람들의 얼굴 데이터셋을 바탕으로, 이를 연령, 성별로 나누는 분류 모델을 학습 및 생성해보는 데 목표가 맞추어져 있습니다. 아시아인, 특히 동북아시아인의 경우에는 생각보다 성별과 연령을 정확히 유추하는 데에 큰 어려움이 있습니다. 본 프로젝트에서는 이런 분류 문제를 해결하기 위해 `Custom Dataset`을 구축하고 이를 개선하려 하였습니다.

### Review
이미지 분류 문제 해결에 있어서 데이터의 절대적 중요성은 아무리 강조해도 부족함이 없습니다. 팀에서는 최초 제시된 데이터셋의 클래스 정보를 편집하고 재분류하였고, 새로운 외부 데이터셋을 보강하여 분류 문제에 있어서 정확도를 개선하려 하였습니다.

최종적으로, 전체 데이터로 10,000장 이상의 얼굴 데이터를 사용하였으며, 최초 모델 대비 비용(용량 등 | `748MB --> 107MB`)적인 부분에서는 큰 개선점을 찾을 수 있었으나, 분류 모델의 성능 자체에서는 `Test Dataset` 대상으로 `70 ~ 75%`의 정확도를 얻을 수 있었습니다.