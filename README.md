# 국회 회의록 분석입니다.  
  
국회 회의록 속기를 분석해 특정 단어들의 출현 빈도를 알아봅니다.  
순서는 아래와 같습니다.  
  
  1. hwp형식의 속기록을 txt로 변환
  2. 문장별로 나눠 데이터프레임 생성
  3. 단어 출현빈도 검색
  4. csv로 저장

---
hwp의 txt변환은 pyhwp를 이용했습니다.  

anaconda prompt:  
  1. pip install pyhwp  
  2. cd로 파일이 있는 폴더로 이동  
    * 예) cd data  
  3. hwp5txt "회의록.hwp" --output "meeting_log.txt"  
    * 단 표나 그림은 <표>,<그림> 등으로 출력됩니다.  
    
참고: [공식문서](https://pyhwp.readthedocs.io/en/latest/converters.html#hwp5txt-text-conversion)
