<img src="https://github.com/user-attachments/assets/25357e11-c0bd-4940-8f97-4b90bc59cee1" border="none">

## ☑️ 프로젝트 개요
통계청과 맥킨지 보고서에 따르면, 대한민국의 출산율은 지속적으로 감소하고 있지만, 자녀수가 줄어들수록 자녀 한 명에게 더 많은 투자를 하는 경향이 나타나고 있습니다. 이로 인해 키즈 산업 시장의 규모는 꾸준히 성장하고 있습니다. 

#### ✔️ 직접 실시한 설문조사
<img src="https://github.com/user-attachments/assets/f1f5137a-98a4-48aa-9957-68931c53f499" width="600px"/>

저희 팀원들은 위와 같이, 현재 육아를 하고 계시는 분들의 의견을 들어보기 위해 구글 폼을 통해 설문조사를 진행해봤었는데요,

<img src="https://github.com/user-attachments/assets/257d33a0-29d4-4533-b22b-e027c802bbf3" width="600px"/>

위의 이미지는 저희가 진행한 설문조사 결과의 일부입니다. 저희는 해당 설문조사를 통해 육아에 할애할 시간이 부족하다는 학부모님이 많다는 걸 확인할 수 있었습니다. 그래서 저희는 3-7세 미취학 아동들이 반복적으로 즐겨하는 역할놀이를 AI가 대신 해줄 수 있다면, 부모님의 육아 부담을 크게 줄일 수 있을 것이라는 생각에 'AI와 함께하는 역할놀이 서비스'를 설계하였습니다.

## ☑️ 프로젝트 진행 기간

> 2024.03.07 - 2024.06.13 : 기획 및 디자인 (동국대학교 기업 연계 캡스톤 디자인 수업)<br/>
> 2024.06.29 - 2024.08.30 : 개발 (LINC 3.0 사업단 산학교육센터에서 진행하는 동국대학교 캡스톤디자인 밸류업)


## ☑️ 팀원 소개
> 팀명: 상쓰리<br/>
> 팀명 의미: 주어진 기회에 대해 모든 상을 휩쓸겠다는 열정으로 임하자!

![image](https://github.com/user-attachments/assets/2a6b1641-fc80-4c24-88cf-81f6578a3f48)

## ☑️ 목차
- [기술 스택](#️-기술-스택)
- [프로젝트 진행 기록](#️-프로젝트-진행-기록)
- [피그마 시안](#️-피그마-시안)
- [ERD](#️-erd)
- [시연 영상](#️-시연-영상)
- [AI 응답 환경 구축](#️-ai-응답-환경-구축)
- [Base Model 선택](#️-base-model-선택)
- [커스텀 데이터셋의 준비](#️-커스텀-데이터셋의-준비)
- [모델 학습 및 프롬프트 조정](#️-모델-학습-및-프롬프트-조정)
- [데이터 통신(서버⇔프론트)](#️-데이터-통신서버프론트)
- [서비스의 이해 & 추후 발전 가능성](#️-서비스의-이해--추후-발전-가능성)
- [아쉬웠던 점](#️-아쉬웠던-점)
- [수상(1)](#️-수상1)
- [수상(2)](#️-수상2)
  
## ☑️ 기술 스택
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)<br/>
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![CSS Modules](https://img.shields.io/badge/CSS_Modules-000000?style=for-the-badge&logo=css-modules&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)<br/>
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=google-colab&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-000000?style=for-the-badge&logo=chainlink&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFB30B?style=for-the-badge&logo=huggingface&logoColor=white)
![LM Studio](https://img.shields.io/badge/LM_Studio-000000?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAEbSURBVHjarJK9SgNBFIW/WZMNwcIiEJsUgq1gI1iJnY2VD2BjYeEL+Bw+gZWNVVr7NBYiFlFIZUgR3FUSdq+FG1lCNpCBU907c+43Z+6Mioh+YX8Dz8AUcAzkkrTwxvMbsA+cADfAFfBRZEhEOiLyICJbIjIvIqsiMiciCyLSFJFTEVkrPsxMzawDnAEHwDKw4u7fZrYPXAPvQM/dv/6MB+4+MLMz4BHouvtvwTezA+AeWHP3p5jZCHgBUmAzxtgzs13gDlh098GYOOecu3vq7kngDngFVoE2MFOIJwZqZqfALXDu7mMgufsTsAOcA9tAIzezVWAD6Lj7MCFHZpYCaYxxOHYVM0vMrFmulFRE5LKsclwWvwMAHrFNi0nCcgMAAAAASUVORK5CYII=)

## ☑️ 프로젝트 진행 기록
<details>
   <summary>✏️ [2024.07.01 - 2024.07.06] week1</summary>
   <br/>
   <table>
     <tr>
       <th>이유정</th>
       <td>- LLM모델에 커스텀 데이터셋 파인튜닝하여 HF에 모델 업로드</td>
     </tr>
     <tr>
       <th>서미영</th>
       <td>- 프론트엔드 테스트 페이지 제작(React)</td>
     </tr>
     <tr>
       <th>이정수</th>
       <td>- 백엔드 API 설계(Spring Boot)</td>
     </tr>
     <tr>
       <th>홍보영</th>
       <td>- 백엔드 DB 설계(Spring Boot)</td>
     </tr>
   </table>
</details>

<details>
   <summary>✏️ [2024.07.07 - 2024.07.12] week2</summary>
   해당 기간동안은 개발 방식에 대해서 아직 구체화되어있지 않은 상황이라, 어떤식으로 개발을 하면 좋을지 공부했습니다.<br/><br/>
   <table>
     <tr>
       <th>이유정</th>
       <td>
         - 개발 방법 모색<br/>
         - HF형식의 모델을 GGUF형식으로 변환해서 HF에 업로드
       </td>
     </tr>
     <tr>
       <th>서미영</th>
       <td>
         - 개발 방법 모색<br/>
         - 리액트 페이지, fastAPI, LM Studio간의 연결 시도
       </td>
     </tr>
     <tr>
       <th>이정수</th>
       <td>- 개발 방법 모색</td>
     </tr>
     <tr>
       <th>홍보영</th>
       <td>- 개발 방법 모색</td>
     </tr>
   </table>
</details>

<details>
   <summary>✏️ [2024.07.13 - 2024.07.21] week3</summary>
   <br/>
   <table>
     <tr>
       <th>이유정</th>
       <td>
         - 대화모델 학습 및 성능 개선 시도
       </td>
     </tr>
     <tr>
       <th>서미영</th>
       <td>
         - 대화모델 연결 및 환경 구축 시도
       </td>
     </tr>
     <tr>
       <th>이정수</th>
       <td>- 보이스 클로닝 구현 방법 모색</td>
     </tr>
     <tr>
       <th>홍보영</th>
       <td>- 역할놀이 결과 페이지 구현 방법 모색</td>
     </tr>
   </table>
</details>

<details>
   <summary>✏️ [2024.07.22 - 2024.07.28] week4</summary>
   <br/>
   <table>
     <tr>
       <th>이유정</th>
       <td>
         - 대화모델 학습 및 성능 개선 시도<br/>
         - 모델 정확도를 높히기 위한 데이터 증강 시도
       </td>
     </tr>
     <tr>
       <th>서미영</th>
       <td>
         - 대화모델 성능 비교 in LM Studio<br/>
         - user의 상황 세부 설정에 따라 다른 프롬프트 연결 시도
       </td>
     </tr>
     <tr>
       <th>이정수</th>
       <td>
         - 보이스 클로닝 구현 방법 모색<br/>
         - OpenVoice 사용 시도
       </td>
     </tr>
     <tr>
       <th>홍보영</th>
       <td>
         - 역할놀이 결과 페이지 구현 방법 모색<br/>
         - Chat-gpt Open API를 사용하여 분석 데이터 얻어내기
       </td>
     </tr>
   </table>
</details>

<details>
   <summary>✏️ [2024.07.29 - 2024.08.04] week5</summary>
   <br/>
   <table>
     <tr>
       <th>이유정</th>
       <td>
         - eeve 모델 훈련 시도<br/>
         - 라마3 모델을 증강된 데이터셋으로 훈련하기<br/>
         - 모델이 상관없는 것까지 길게 출력하는 문제 해결 시도<br/>
         - 모델 수치적으로 평가하는 방법 찾아보기<br/>
         - 입력 문장 여러 개일 경우 응답 확인
       </td>
     </tr>
     <tr>
       <th>서미영</th>
       <td>
         - 쿼리스트링 방식말고 body에 담아서 json형태로 fastAPI 서버에 사용자의 선택 정보 전달하기 (API 연결)<br/>
         - 기획 구체화 (서비스적인 측면에서)
       </td>
     </tr>
     <tr>
       <th>이정수</th>
       <td>
         - voice cloning 실제 서버에 올려서 테스트 페이지에서 사용가능하게 조작<br/>
         - 생성한 tts를 저장하여 사용할 수 있는 방법 찾기
       </td>
     </tr>
     <tr>
       <th>홍보영</th>
       <td>
         - 백앤드 기능 필요한 거 crud 코드 전부 완성하기 -> 연결부분 빼고 모두 작동할 수 있도록 만들기<br/>
         - 결과분석 api 부모들이 더 신뢰할 수 있을 만한 내용을 제공할 수 있는 방안 모색하기 -> 프롬프트 템플릿화<br/>
         - api 명세 다시 구체화하기<br/>
         - 결과분석 페이지를 디자인해서 오기 (결과 분석 페이지 UI)
       </td>
     </tr>
   </table>
</details>

<details>
   <summary>✏️ [2024.08.05 - 2024.08.09] week6 </summary>
   <br/>
   <table>
     <tr>
       <th>이유정</th>
       <td>
          - 모델 전반적인 학습<br/>
          - 모델 크기 감소 시도<br/>
       </td>
     </tr>
     <tr>
       <th>서미영</th>
       <td>
          - 모델 응답이 혼자서 시나리오를 짜는 걸 막기<br/>
          - 쿼리스트링 방식말고 body에 담아서 json형태로 fastAPI 서버에 사용자의 선택 정보 전달하기 (API 연결)<br/>
          - 사용자 입장에서 응답이 완성될때까지 기다리기 너무 힘드니깐, 모든 응답이 완성되지 않더라도, 생성되는대로 한글자씩 화면에 순차적으로 띄우기 => 힘들면, 응답이 완성되는 동안 '응답 생성 중...'이라는 로딩 표시라도 띄우기
       </td>
     </tr>
     <tr>
       <th>이정수</th>
       <td>
          - OpenVoice와 berk를 이용한 보이스 클로닝 시도<br/>
          - 일반 TTS: Melo(OpenVoice를 개발한 개발팀과 같은 팀이며, local로 설치하여 사용할 수 있는 리눅스 기반의 오픈소스 TTS) 사용 시도<br/>
       </td>
     </tr>
     <tr>
       <th>홍보영</th>
       <td>
          - 지난주에 이어서, 결과 분석 페이지 개발 진행<br/>
       </td>
     </tr>
   </table>
</details>

<details>
   <summary>✏️ [2024.08.10 - 2024.08.18] week7 </summary>
   <br/>
   <table>
     <tr>
       <th>이유정</th>
       <td>
          - [영상공모전] 영상 편집 및 준비<br/>
          - 베이스 모델을 EEVE모델로 변경해서 재파인튜닝<br/>
          - 장난감에 맞는 데이터셋을 추가
       </td>
     </tr>
     <tr>
       <th>서미영</th>
       <td>
          - [영상공모전] 준비<br/>
          - 프론트엔드 전반적인 작업 마무리(페이지 작업 및 서버와 API연결)<br/>
          - 그동안 Web Speech API로 제공했던 TTS를, Google의 TTS API와 연결
       </td>
     </tr>
     <tr>
       <th>이정수</th>
       <td>
          - [영상공모전] 영상 편집, 디자인 및 준비<br/>
          - 보이스 클로닝 시도
       </td>
     </tr>
     <tr>
       <th>홍보영</th>
       <td>
          - [영상공모전] 준비<br/>
          - 백엔드 전반적인 작업 마무리(API설계 및 DB구축)<br/>
       </td>
     </tr>
   </table>
</details>

## ☑️ 피그마 시안
![image](https://github.com/user-attachments/assets/0845c2d2-8450-4a85-b9f7-474c81a2ea42)

## ☑️ ERD
![image](https://github.com/user-attachments/assets/a16fdb9c-84f6-49b5-8c1d-9989ba5a8cd4)
참고로, 해당 ERD에는 '사용자'에 대한 정보가 저장되도록 했지만, 실제 테스트 웹페이지에서는 사용자를 임의로 지정하고 진행했습니다.

## ☑️ 시연 영상
https://github.com/user-attachments/assets/bf1a59a5-042b-49e0-96ab-69055721608b
#### ✔️ LLM 파인튜닝을 통한 나만의 언어모델
한국어 성능이 우수한 EEVE모델을 기본 모델로 선정했습니다. 커스텀 데이터셋을 직접 구축했고, 성능 최적화를 위해 BERT모델을 활용한 데이터셋 증강 및 파인튜닝을 진행했습니다.

#### ✔️ 음성 기반의 역할놀이 서비스: 아이들의 새로운 친구 '아고미'
STT(Web Speech API)와 TTS(Google TTS API) 기술을 활용해 음성 기반 역할놀이를 제공했습니다. '아고미'라는 마스코트 캐릭터를 중심으로 다양한 캐릭터를 제작해, 사용자가 원하는 캐릭터의 음성을 선택하여 역할놀이를 진행할 수 있도록 했습니다.

#### ✔️ 역할놀이 결과 분석 레포트 제공
GPT-3.5-Turbo를 활용하여 결과 분석 레포트를 제공함으로써, 부모님들이 역할놀이에 직접 참여하지 않고도, 아이들의 역할놀이를 효과적으로 파악할 수 있게 했습니다.

## ☑️ AI 응답 환경 구축
#### ✔️ AI의 응답을 받아오는 방법에 대한 다양한 고민들
다음 링크에 포함된 글들을 참고해주세요.
- [LM Studio의 사용 + ngrok, fastAPI](https://github.com/Prize-Three/record/issues/1)
- [Hugging Face Transformers방식](https://github.com/Prize-Three/record/issues/4)
- [꼭 LM Studio를 사용해야만 할까?](https://github.com/Prize-Three/record/issues/5)
- [코랩에서 모델 크기 관련 이슈](https://github.com/Prize-Three/record/issues/8)
- [코랩 환경 테스트](https://github.com/Prize-Three/record/issues/12)
- [Ollama구동시도](https://github.com/Prize-Three/record/issues/13)
- [모델 응답이 혼자서 시나리오를 짜는 걸 막기](https://github.com/Prize-Three/record/issues/23)

#### ✔️ LM Studio의 사용
저희 팀은 모델을 효과적으로 테스트하고 실제 환경에서 사용하기 위해 LM Studio라는 프로그램을 이용했습니다.
LM Studio를 선택하기로 결정한 데에는 다음과 같은 이유가 있습니다.
1. 제한적인 GPU자원
   - 대규모 언어 모델을 실행하려면 보통 강력한 GPU가 필요한데 저희에게는 그런 고성능 장비가 충분하지 않았습니다. 그래서 LM Studio라는 프로그램을 사용하면, 일반 컴퓨터에서 그나마 대형 언어 모델을 비교적 쉽게 돌릴 수 있을 것이라는 생각에 사용하게 되었습니다.
2. 짧은 프로젝트 기한
   - 저희는 개발 기간이 기획 기간에 비해 상대적으로 짧았기 때문에 시간이 없었습니다. 그래서 모델의 성능을 빠르고 효율적으로 테스트할 수 있는 환경이 필요했습니다. LM Studio는 사용자 친화적인 인터페이스를 제공하기 때문에 크게 복잡한 설정 없이도 모델을 쉽게 로드하고 성능을 테스트할 수 있습니다.
3. 저장 공간 절약
   - 모델을 로컬에 직접 다운로드 하지 않아도 된다는 점이 큰 장점이었습니다. 보통 대형 언어 모델은 용량이 매우 크기 때문에 이 점은 큰 장점으로 다가왔습니다.

## ☑️ Base Model 선택
저희팀은 프로젝트를 시작하면서 어떤 대형 언어 모델(LLM)을 기반으로 파인튜닝을 진행할지 많은 고민을 했습니다. 

많은 모델들을 비교해보기에는 현실적인 제약이 있었습니다. 바로 GPU 자원의 한계였는데요, 이런 대규모 언어 모델들을 훈련시키고 테스트하려면 엄청난 컴퓨팅 파워가 필요한데, GPU가 없는 상태에서는 학습에 제한이 있었습니다. 한번 테스트 하는데 많은 시간과 비용이 소모되기 때문에 다양한 모델을 테스트 해보는 건 현실적으로 불가능했습니다. 그래서 어쩔 수 없이 선택과 집중을 해야했고, 저희는 META, LLAMA3, EEVE 이 세 모델을 우선적으로 선택했습니다.

#### ✔️ LM Studio에서 직접 실행시켜서 성능 비교
- 세 모델을 gguf형식으로 변환한 모델을 비교했습니다.
   - Q. 왜 gguf형식으로 변환하나요?
      - A. LM Studio는 gguf형식(모델을 압축해서 더 효율적으로 사용할 수 있게 만든 파일 형식)의 모델만 인식가능하기 때문입니다.
   - 상쓰리 HuggingFace계정에 올려놓은 GGUF 모델들
      - (1) [라마3 기반](https://huggingface.co/sangthree/0707_gguf)
      - (2) [META 기반](https://huggingface.co/sangthree/meta_0706_gguf)
      - (3) [EEVE 기반](https://huggingface.co/sangthree/final_eeve_gguf)
   - LM Studio내에서 직접 성능을 비교한 결과
      - [모델 성능 비교 in LM Studio](https://github.com/Prize-Three/record/issues/15)

=> 결론적으로 EEVE를 Base Model로 선택하였습니다. EEVE는 한국어 처리에 더 특화되어있고, 복잡한 지시사항을 더 잘 이해할 수 있는 모델입니다.

## ☑️ 커스텀 데이터셋의 준비
일단 저희가 모든 역할놀이 구성에 대한 데이터셋을 다 구성할 수는 없었기에 2가지 상황을 대표로 정하고 커스텀 데이터셋을 구성했습니다.
(상황1) 사용자-의사, AI-환자
(상황2) 사용자-요리사, AI-손님

#### ✔️ [STEP1] 초반 데이터셋의 준비
처음에는 (상황1)에 대한 데이터셋만 준비한 상황이었습니다.
- [Hugging Face에 올린 초반 데이터셋](https://huggingface.co/datasets/sangthree/hospital_1)

#### ✔️ [STEP2] 데이터셋 증강
- [증강 관련 이슈](https://github.com/Prize-Three/record/issues/18)

#### ✔️ [STEP3] 데이터셋 구조 변화
- [Hugging Face에 올린 변화된 데이터셋](https://huggingface.co/datasets/sangthree/new_hospital_situation)
  
저희팀이 처음 프로젝트를 시작했을 때는 META와 LLAMA3를 기반으로 파인튜닝을 진행했었습니다. 해당 모델들은 모두 입력(input)을 받아, 응답(response)을 생성하는 방식으로 작동하기 때문에 기존에 저희가 [STEP1]에서 준비했던 커스텀 데이터셋의 형태가 적합했습니다. 

하지만, 프로젝트를 진행하면서 성능을 향상시키기 위해 베이스 모델을 EEVE로 변경하였습니다. 이런 변경에 맞춰서 자연스럽게 데이터셋의 구조도 변경해야했었습니다. 파인튜닝을 위해 기존의 (’input’, ‘response’에서 ‘instruction’,’output’,’input’)으로 재구축했습니다. EEVE 모델의 데이터셋 구조가 instruction , output, input으로 이루어져있기 때문에 파인튜닝을 위한 필수 과정입니다. instruction 필드에는 대화에서 필요한 질문을 명확히 제시하고, output필드에는 모델이 생성해야 할 응답을 포함했습니다. input필드는 instruction만으로도 충분한 정보를 제공할 수 있다고 판단하여 비워놓았습니다. input을 채워두면 특정 입력 패턴에 과도하게 의존할 수 있습니다. 역할놀이 대화 챗봇의 경우 다양한 상황에 유연하게 대응할 필요가 있다고 판단하여 input을 비우는게 성능상에서 더 효과적일것이라고 생각했습니다.

#### ✔️ [STEP4] 최종 데이터셋
- [Hugging Face에 올린 최종 데이터셋](https://huggingface.co/datasets/sangthree/FinalDatasets)
  
##### (1) 장난감 세트에 맞춤 커스텀 데이터 셋 추가
예를 들어 아이들이 사용하는 장난감에 파란색과 빨간색 밴드가 있다고 합시다.
![image](https://github.com/user-attachments/assets/e6ddc0a7-2879-4fa6-92eb-e7d138a903ed)
이렇게 예상되는 질문과 응답에 대한 커스텀 데이터셋을 추가했습니다. 

##### (2) (상황2: 요리놀이)에 대한 데이터셋 추가
기존에는 (상황1: 병원놀이)에 대한 데이터셋만 있었는데 추가했습니다.
![image](https://github.com/user-attachments/assets/04ce54be-e6e2-4488-ade7-a9effe9b81a8)


## ☑️ 모델 학습 및 프롬프트 조정
> 모델의 학습 코드는 다음 레포지토리에 모아져있습니다.
> - [model 레포지토리 이동](https://github.com/Prize-Three/model)

> 프롬프트 명령어 설정
> - [프롬프트에 따른 답변 변화 확인](https://github.com/Prize-Three/record/issues/16)

#### ✔️ 간단 설명
##### (1) LoRA방식의 파인튜닝
저희는 LoRA(Low-Rank Adaption) 방식으로 모델을 파인튜닝했습니다. 이 방법은 전체 모델의 파라미터를 수정하지 않고 일부만 업데이트하여 효율적으로 학습할 수 있게 해줍니다. 이를 통해 적은 자원으로도 빠르게 원하는 성능을 얻을 수 있습니다.

##### (2) 상황에 따른 프롬프트 
실제 서비스 구현 단계에서는 LM Studio를 활용하여 모델의 응답을 생성했습니다. 이 과정에서 저희는 프롬프트 엔지니어링 기법을 적용했습니다. 즉, 상황에 따라 다양한 프롬프트를 동적으로 구성하여 모델에게 전달함으로써, 원하는 역할과 맥락에 맞는 응답을 유도했습니다.

이러한 접근 방식을 통해, 저희는 효율적으로 학습된 모델을 기반으로 하면서도, 프롬프트 조정을 통해 다양한 상황과 역할에 유연하게 대응할 수 있는 시스템을 구축했습니다.

## ☑️ 데이터 통신(서버⇔프론트)
#### ✔️ 주고받는 데이터 형식
- [주고받는 데이터의 형태(json)](https://github.com/Prize-Three/record/issues/27)
- 서버에 정보 전달 방법
   - [JSON --> 채택](https://github.com/Prize-Three/record/issues/25)
   - [쿼리스트링 --> 미채택](https://github.com/Prize-Three/record/issues/17)

#### ✔️ 대화형 API 문서 페이지(http://localhost:8000/docs)
<details>
   <summary>[확인]</summary>
   <img src="https://github.com/user-attachments/assets/d847a9fd-d8df-4cbf-9794-b60caedaa4c6"/>
</details>

#### ✔️ 연결 방식
> 참고로 Fetch API는 클라이언트측에서 제공하는 네트워크 요청을 보내기 위한 인터페이스입니다. 그리고 RESTful API는 서버 측에서 구현된 API의 설계 원칙입니다.

React코드에서는 Fetch API를 사용하여 RESTful API와 통신하고 있습니다. Fetch API는 RESTful API를 호출하기 위한 도구로 사용되고 있습니다. 

## ☑️ 서비스의 이해 & 추후 발전 가능성
![image](https://github.com/user-attachments/assets/33c289a6-502f-4c72-9e67-5b2ec036020d)
해당 서비스는 화면을 보면서 하는 역할놀이가 아니라, 음성 보조 역할을 하는 서비스입니다. 
부모님께서 아이들한테 역할놀이에 대답해 줄 여유가 없을때에 대신 답변해줄 수 있는 서비스입니다.

현재는 음성 기반으로만 구현되어있습니다. 아이들의 발화를 STT를 통해 텍스트로 얻어오고, 그에 대한 응답을 LLM모델을 통해 생성해낸 뒤, TTS로 아이들한테 응답하는 과정이 구현되어있습니다. 

저희는 해당 서비스를 장난감 사업으로 확장할 수 있다고 생각합니다. 다양한 역할놀이 상황에 대한 장난감들을 판매하고, 아이들은 해당 장난감을 가지고 놀면서 역할놀이를 진행합니다.

현재는 아이들의 발화 정보만을 가지고 응답을 생성해내지만, 추후에 해당 서비스가 발전한다면, 장난감에 센서를 부착하여 아이들이 어떤 장난감을 가지고 노는지에 대한 데이터도 얻어서, 음성 데이터 뿐만 아니라 센서 데이터도 고려해 응답을 생성하면 더 나은 서비스가 될 것이라고 생각했고, 현재 이런 서비스적인 부분에 관련된 특허 출원을 하려고 진행중입니다.

## ☑️ 아쉬웠던 점
### ✔️ 1. 다중 사용자 지원
현재는 단일 사용자와 AI간의 1:1 대화만 지원하지만, 다중 사용자 환경에서의 대화 처리 기능을 구현하는 식으로 개선하면 더 나은 서비스가 될 것이라고 생각합니다.

### ✔️ 2. 동적 대화 생성
현재는 사용자의 하나의 발화당 AI의 단일 응답을 생성하나, 상황에 따라 유동적으로 2-3개의 응답을 생성하는 지능형 대화 시스템이 구현되어야 된다고 생각합니다.

### ✔️ 3. 응답 생성 시간이 너무 오래 걸림
사실 이 문제는 GPU의 문제가 큽니다. 훨씬 가벼운 모델로 다시 테스트하거나, 좋은 성능의 하드웨어를 사용하거나, 양자화 기법을 사용하여 모델의 크기를 축소할 수 있다고 생각합니다.

#### (1) 가벼운 모델로 고려사항
- [모델 링크](https://github.com/Beomi/KoAlpaca/tree/main)
  
#### (2) 경량화를 위한 양자화 기법은 6가지 정도
 1) 정적 양자화
     가중치와 활성화를 더 작은 비트로 변환하는 방식
     장점: 빠르게 구현할 수 있을 정도로 간단/모델 크기를 크게 줄일 수 있음/추론 속도를 향상시킬 수 있음
     단점: 정확도 손실 가능성/ 동적 범위가 큰 데이터에 취약
                    
  2) 동적 양자화
     추론 타이밍에 활성화를 동적으로 양자화하는 방식으로 가중치는 정적으로 양자화 됩니다.
     장점: 구현이 비교적 간단/ 활성화의 동적 범위 처리 가능/ 메모리 사용량 감소시킬 수 있음
     단점:  정적 양자화보다 추론 속도가 느릴 수 있음/ 실시간 계산을 하기 때문에 이로 인한 오버헤드 발생 가능성이 있음/ 일부 연산에서 정확도 손실 가능성이 있음

  3) 양자화 인식학습
     학습의 단계에서 양자화 효과를 시뮬레이션하는 방식으로 좀 더 높은 정확도를 만들 수 있지만 추가학습이 필요합니다. 
     장점: 높은 정확도 유지가 가능/양자화 효과를 학습에 반영할 수 있음/최종 모델의 성능이 향상 되는 효과
     단점: 추가적인 학습 시간 필요/구현이 복잡/계산 리소스 요구량이 많음 

 4) 프루닝과 양자화 결합
    불필요한 가중치를 제거하고 양자화를 적용하는 방식
    장점: 모델 크기와 복잡성이 감소/불필요한 파라미터 제거 -> 효율성이 향상됨/양자화와 시너지 효과를 낼 수 있음
    단점: 구현이 복잡/프루닝 정도 설정에 주의가 필요함/과도한 프루닝 시 성능 저하의 가능성이 있음
 
 5) 혼합 정밀도 훈련
    일부의 연산은 낮은 정밀도로 다른 연산은 높은 정밀도로 수행하는 방식
    장점: 학습 속도 향상/메모리 사용량 감소/높은 정확도 유지 가능
    단점: 하드웨어를 타는 경향이 있음/구현이 조금 복잡할 수 있음/결과 안정성 문제가 발생할 가능성이 있음
 
 6) 지식증류
    큰 모델의 지식을 작은 모델로 전달하는 방식
    장점: 작은 모델로 큰 모델의 성능을 낼 수 있음/모델 크기가 대폭 감소됨/일반화 성능 향상 가능
    단점: 교사 모델 선택 및 학습에 시간이 꽤 소요되고 구현이 복잡할 수 있고 학생 모델 아키텍쳐 설계에 세심한 주의가 필요함
    
### ✔️ 4. RAG를 사용하지 못한 점
GPU문제를 해결하기 위해서 RAG를 도입할 수 있다고 생각한다. 사실 프로젝트 초반에는 역할놀이와 관련된 별도의 PDF 자료를 준비할 필요가 없다고 판단하여 RAG를 사용하지 않기로 결정했었다. 그러나 프로젝트 후반부에 갈수록 큰 모델에 대한 문제점을 해결하기 위해 어쩌면 RAG를 사용할수도 있겠다는 생각이 들었다. 정말 많이 예상되는 질문은 RAG로 구성해서, 랭체인으로 모델의 응답을 받아오기 전에 RAG선에서 끝내는 것이다. 그러면 뻔한 대답은 금방 답변을 받을 수 있을것이라고 생각했습니다.

## ☑️ 수상(1) 
> SK텔레콤과 동국대학교가 공동으로 주관한 2024년 1학기 「기업사회맞춤형캡스톤디자인」에서 교과우수상 수상

저희는 skt의 서비스와 관련시켜서, 해당 서비스 개발을 진행했습니다. 많은 skt의 서비스 중에서도 '에이닷'이라는 서비스를 어떻게 개선시킬지를 고민했는데요, 결론만 말하자면 에이닷의 서비스의 메인 서비스가 뚜렷하지 않다고 생각했습니다. 즉, 타겟층도 뚜렷하지 않다고 생각했습니다. 그래서 '키즈 플랫폼'을 에이닷의 메인 서비스로 내세우면 에이닷을 알릴 수 있을 것이라고 생각했고, 저희는 인공지능을 활용해, 키즈 플랫폼에 들어갈만한 서비스를 개발하게 되었습니다. 기획적인 부분들에 대해 세세하게 듣고 싶으시다면, 다음 발표 영상을 참고해주세요. <br/><br/>
✔️ 최종 발표 영상: https://youtu.be/5XKj9iJxWFw<br/>
✔️ 질의 응답 영상: https://youtu.be/Lr1ReEtKcho

## ☑️ 수상(2) 
> 동국대학교 산학교육센터가 주관한 「2024 CD 59초 영화제」 최우수상 수상

https://github.com/user-attachments/assets/bf985856-7ed0-40f1-a82a-0381921dee49
