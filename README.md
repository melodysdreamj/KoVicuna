<p align="center" width="100%">
<img src="assets/logo.png" alt="KoVicuna icon" style="width: 200px; height:200px; display: block; margin: auto; border-radius: 50%;">
</p>

## Update Logs

- 2023.4.20: [🤗LLAMA 7B 기반 KoVicuna 모델](https://huggingface.co/junelee/ko_vicuna_7b) 을 공개합니다.

---

# KoVicuna: Korean Vicuna Model based on Vicuna (feat. LLAMA)

Vicuna 모델을 학습한 방식과 동일한 방식과 모델셋으로 학습을 진행한, 한국어 Vicuna 모델입니다.


## 예시

<img width="742" alt="스크린샷 2023-04-20 오후 12 59 37" src="https://user-images.githubusercontent.com/21379657/233285899-57e350b1-c0cd-4a5d-95e2-dda2376d2947.png">


## 데이터셋 제작 방법

데이터셋은 기본적으로 [ShareGPT 제공한 62만 대화문 데이터셋](https://huggingface.co/datasets/anon8231489123/ShareGPT_Vicuna_unfiltered)을 기반으로 합니다.

해당 대화문을 DeepL 을 통해 모두 번역했습니다. [번역본 링크](https://huggingface.co/datasets/junelee/sharegpt_deepl_ko)

## 학습경과

1. 번역된 62만 대화문과 Vicuna 7B 를 준비
2. A100 * 8 개로 15시간 동안 학습 진행
3. 자세한 학습 내역은 [이곳](https://github.com/melodysdreamj/KoVicuna/blob/main/assets/KoVicuna%20training%20Report%20_%20huggingface%20%E2%80%93%20Weights%20%26%20Biases.pdf)을 참고해주세요.

<img width="300" alt="W B Chart 2023  4  20  오후 3_57_14" src="https://user-images.githubusercontent.com/21379657/233285808-f6e5514a-107a-4392-ac21-2ea631fce2c2.png">


## 데모

### 1. 코랩
코랩프로일 경우 코랩에서 바로 사용해 보실수 있습니다.

이 [주소](https://colab.research.google.com/drive/1EOFuhdkE5IjRKaSZOZDwhDicXU1cUE5f?usp=sharing)를 통해 코랩에 들어간후 자세한 가이드를 따라해주세요.


### 2. 우바부가 (text-generation-webui)
해당 모델은 비쿠나1.1v으로 학습되었으므로 우바부가를 사용할경우 Character 탭 에서 다음을 설정해주세요.
  1. Your name -> USER: 
  2. Character's name -> ASSISTANT: 

## 가중치공개

- 준의 허깅페이스에서 [가중치](https://huggingface.co/junelee/ko_vicuna_7b) 를 확인할 수 있습니다.



### Author
- [JUNE LEE](https://github.com/melodysdreamj) - [송도 인공지능 스터디](https://open.kakao.com/o/gUEN1NK)에서 활동하고 있습니다.
