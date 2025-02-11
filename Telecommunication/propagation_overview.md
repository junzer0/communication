## 1.1 전파 이론
### 1.1.1. 전파의 특성
- 전파 지연, 전파 손실, 전파 간섭, 도플러 효과
### 1.1.2. 전파 지연
- Propagation delay = distance / propagation speed
- 패킷 통신 시스템에서의 지연
    1) Access delay
	2) Processing delay
	3) Queueing delay
	4) Transmission delay
	5) Propagation delay
### 1.1.3.전파 손실
- 전파의 거리: 거리가 증가함에 따라 전파 에너지가 퍼져 손실이 발생
	1) 거리 손실(Path loss)
	2) 전파 감쇄(Propagation loss)
- 지형 및 장애물: 전파가 장애물을 만날 때, 투과하지 못하고 반사되거나 산란되어 손실 발생
- 주파수: 고주파에서 작동하는 이동통신 시스템은 대기 상의 산란 및 흡수 등으로 손실이 큼
	  
![전파 손실의 변동성 비교(출처_정보통신기술용어해설)](https://github.com/junzer0/communication/blob/main/img/propagation_loss.png)

1) 프리스-하탁 모델: 프리스 전송 방정식을 바탕으로 공간적 분산 및 채널 특성을 기반으로 하는 전파 손실 모델
	    - 단점: 국소 환경의 영향을 고려하지 않음 -> 실제 전파 손실을 정확하게 예측 어려움
	    - 실제 전파 손실을 예측하기 위해서는 경로 손실 모델, 섀도잉 및 다중 경로 페이딩 등의 다른 전파 모델들을 함께 고려해야 함
2) 오쿠무라-하타 모델: 실외 환경 전파 모델(인간주거환경을 고려하여 측정된 데이터의 체계적인 해석에 의해 제안된 ‘경험적 전파모델’)
3) Walfish-Ikegami 모델
- 자유 공간 손실(Free Space Loss): 이상적인 자유 공간에서 송수신 수신 강도를 예측하기 위해 사용(거리만 고려) 
    - 위성통신, 고정 점대점 M/W(Micro Wave) 통신
### 1.1.4. 전파 간섭
- 이동통신 시스템에서 발생하는 신호 간의 충돌을 말함
### 1.1.5. 도플러 효과
- 수신기와 송신기 간의 상대적 이동 속도 차이로 인해 주파수가 변화하는 현상 
### 1.1.6. 다중 경로 전파
- 전파 신호가 주파수의 특성과 환경 요인에 따라 다양한 경로를 통해 수신기로 도달하는 현상
- 주로 다이버시티를 활용하여 해결
- TDMA -> 등화기 사용, CDMA -> 레이크 수신기 활용

![다중 경로 페이딩](https://github.com/junzer0/communication/blob/main/img/multi-path-fading.png)

## 1.2. 전파와 주파수
- 저주파대역: 600MHz~900MHz(2G, 3G)
- 중주파 대역: 1.8GHz~2.2GHz(2G GSM, 3G UMTS, 4G LTE)
- 고주파 대역: 2.3GHz~2.7GHz(4G LTE-A, 5G NR)
- 초고주파 대역: 24GHz~60GHz(5G mmWave대역)

![전자파의 분류(출처_한국방송통신전파진흥원)](https://github.com/junzer0/communication/blob/main/img/propagation_index.png)

- 전파 전송 모드
  - 협대역(Narrowband)
    - 대역폭: 25kHz 이하
    - 데이터 전송률(bps) 낮음
    - 장거리 전송 가능
    - 잡음에 강함
  - 광대역(Wideband)
    - 대역폭: 25kHz~500kHz
    - 데이터 전송률, 전송 거리, 잡음 중간
  - 초광대역(Ultra-Wideband)
    - 대역폭: 500kHz 이상
    - 짧은 거리 전송
    - 잡음에 약함
    - 에너지 소비량 큼

## 1.3. 간섭 및 잡음
