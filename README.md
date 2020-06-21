# NLP-TP

- <h4>파일 설명</h4>

  - NLP-TP.ipynb: 프로젝트에 필요한 코드가 있는 colab notebook

  - data: nsmc 데이터가 있는 디렉토리

    

- <h4>실행 방법</h4>
  
  - 현재 repository 내에 있는 **NLP-TP.ipynb**를 [google colab](https://colab.research.google.com/)에서 불러와서 실행
    - [google drive](https://drive.google.com/)에 마운트 해서 실행 ([사용한 구글 드라이브](https://drive.google.com/drive/folders/1XfjSPZMtK5hsfbwoIHKwIaYFF3ND3VWQ?usp=sharing))
      - 경로는 `/content/drive/My Drive/course-NLP-TP/`
      - 총 4개의 섹션이 있고, 앞의 3개는 finetuning 모델, 마지막은 [kaggle](https://www.kaggle.com/c/cose461k) 제출을 위해 csv 파일을 제출 형식에 맞춰서 만드는 코드
      - 앞의 3개 섹션은 각 모델별로 섹션을 나눠놓았고, KoBERT, HanBERT, KoELECTRA 모델을 사용. 각 섹션은
        1. github code clone 및 경로 설정
        2. 해당 code 실행에 필요한 dependency 설치
        3. finetuning (training)
        4. prediction
      - 하는 코드 블럭으로 이루어짐
      - KoELECTRA 섹션의 경우, finetuning하는 코드 내에 kaggle data에 대한 prediction을 저장하게 해서, 따로 prediction을 위한 코드 블럭이 없음



- <h4>참고한 소스</h4>

  - [KoBERT](https://github.com/monologg/KoBERT-nsmc)
  - [HanBERT](https://github.com/monologg/HanBert-nsmc)
  - [KoELECTRA](https://github.com/monologg/KoELECTRA)

