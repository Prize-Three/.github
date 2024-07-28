![image](https://github.com/user-attachments/assets/d8cec42c-9606-422b-8161-7f97aa752394)

## 📍 프로젝트 소개
> AI와의 음성 기반 역할 놀이 시스템 

## 📍 개발 기간
> 2024.06.29 - 2024.08.21


## 📍 팀원 소개
> 팀명: 상쓰리

|          [이유정](https://github.com/zlwmxkdla)           |          [서미영](https://github.com/SeoMiYoung)           |          [이정수](https://github.com/Lee-JeongSoo)           |          [홍보영](https://github.com/BoyoungH)           |
| :------------------------------------------------------: | :-----------------------------------------------------: | :-------------------------------------------------------: | :--------------------------------------------------------: |
| ![이유정의 프로필 사진](https://github.com/zlwmxkdla.png) | ![서미영의 프로필 사진](https://github.com/SeoMiYoung.png) | ![이정수의 프로필 사진](https://github.com/Lee-JeongSoo.png) | ![홍보영의 프로필 사진](https://github.com/BoyoungH.png) |

## 📍 WEEKLY PLAN
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
         - 프롬프트 엔지니어링 방식에 대해서 자세히 찾아보기 => 어떻게 하면 최적의 프롬프트를 찾을 수 있을까 찾아보기
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
         - 결과분석 페이지를 디자인해서 오기
       </td>
     </tr>
   </table>
</details>

<details>
   <summary>✏️ [2024.08.05 - 2024.08.11] week6 </summary>
   <br/>
   <table>
     <tr>
       <th>이유정</th>
       <td>
       </td>
     </tr>
     <tr>
       <th>서미영</th>
       <td>
       </td>
     </tr>
     <tr>
       <th>이정수</th>
       <td>
       </td>
     </tr>
     <tr>
       <th>홍보영</th>
       <td>
       </td>
     </tr>
   </table>
</details>

<details>
   <summary>✏️ [2024.08.??] 대면 모임 (사진 촬영) </summary>
   <br/>
   <table>
     <tr>
       <th>이유정</th>
       <td>
       </td>
     </tr>
     <tr>
       <th>서미영</th>
       <td>
       </td>
     </tr>
     <tr>
       <th>이정수</th>
       <td>
       </td>
     </tr>
     <tr>
       <th>홍보영</th>
       <td>
       </td>
     </tr>
   </table>
</details>

<details>
   <summary>✏️ [2024.08.12 - 2024.08.18] week7 </summary>
   <br/>
   <table>
     <tr>
       <th>이유정</th>
       <td>
       </td>
     </tr>
     <tr>
       <th>서미영</th>
       <td>
       </td>
     </tr>
     <tr>
       <th>이정수</th>
       <td>
       </td>
     </tr>
     <tr>
       <th>홍보영</th>
       <td>
       </td>
     </tr>
   </table>
</details>
