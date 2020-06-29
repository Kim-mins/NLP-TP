# NLP-TP

- <h4>파일 설명</h4>

  - NLP-TP.ipynb: 프로젝트에 필요한 코드가 있는 colab notebook

  - data: nsmc 데이터가 있는 디렉토리
    - 아래 참고한 소스에서 이미 nsmc 데이터가 있고 해당 데이터에 대한 전처리 코드도 참고한 소스 내에 모두 포함이 되어있어서, 여기는 raw 데이터만 올립니다.

    

- <h4>실행 방법</h4>
  
  - 현재 repository 내에 있는 **NLP-TP.ipynb**를 [google colab](https://colab.research.google.com/)에서 불러와서 실행
    - [google drive](https://drive.google.com/)에 마운트 해서 실행 ([사용한 구글 드라이브](https://drive.google.com/drive/folders/1XfjSPZMtK5hsfbwoIHKwIaYFF3ND3VWQ?usp=sharing))
      - 경로는 `/content/drive/My Drive/course-NLP-TP/`
    - notebook에는 총 4개의 섹션이 있고, 앞의 3개는 finetuning 모델, 마지막은 [kaggle](https://www.kaggle.com/c/cose461k) 제출을 위해 csv 파일을 제출 형식에 맞춰서 만드는 코드
    - 앞의 3개 섹션은 각 모델별로 섹션을 나눠놓았고, KoBERT, HanBERT, KoELECTRA 모델을 사용. 각 섹션은...
      1. github code clone 및 경로 설정
      2. 해당 code 실행에 필요한 dependency 설치
      3. finetuning (training)
      4. prediction
    - 하는 코드 블럭으로 이루어짐
    - KoELECTRA 섹션의 경우 finetuning하는 코드 내에 kaggle data에 대한 prediction 결과를 fine-tuning 도중에 저장하게 해서, 마지막 섹션에서 따로 prediction을 위한 코드 블럭이 없음
    - 마지막 섹션의 2번째 코드 셀의 경우 finetuning이 완료된 KoBERT, HanBERT 모델을 kaggle data를 통해 prediction하는 작업을 함
      - 현재 노트북에서는, kaggle data의 이름은 ko_data.txt, predict 결과 label이 저장되는파일은 ko_data_out.txt가 됨 (11187줄)
    - 마지막 섹션의 3번째 코드 셀은 3개의 모델 모두가 사용. prediction된 결과를 제출용 csv로 변환하는 파일
      - ex)           Id  Predicted
            1         0   1
            1         1   1
            0     =>  2   0
            0         3   0
            1         4   1
            ...



- <h4>참고한 소스</h4>

  - [KoBERT](https://github.com/monologg/KoBERT-nsmc)
  - [HanBERT](https://github.com/monologg/HanBert-nsmc)
  - [KoELECTRA](https://github.com/monologg/KoELECTRA)

