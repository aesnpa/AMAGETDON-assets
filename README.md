# AMAGETDON-assets

아마겟돈 학습 챕터 본문에 들어가는 이미지 저장소입니다. 코드가 아니라 **정적 파일만** 둡니다.

## URL 규칙

본문(`chapters.csv`의 `chapter_content`)에서는 아래 주소를 `<img src>`에 그대로 씁니다.

```
https://raw.githubusercontent.com/aesnpa/AMAGETDON-assets/main/chapter/<파일명>
```

예시:

```html
<figure>
  <img src="https://raw.githubusercontent.com/aesnpa/AMAGETDON-assets/main/chapter/ch1_01_trade_flow.png"
       alt="주식 거래 흐름">
  <figcaption>주식 거래 흐름</figcaption>
</figure>
```

## 파일명 규칙

```
ch{chapter_id}_{순번}_{내용}.png
```

- `chapter_id` — DB `chapters` 테이블의 기본키. 노션 챕터 번호가 아닙니다.
- `순번` — 해당 챕터 본문에서 위에서부터 몇 번째 이미지인지.

**한글 파일명은 쓰지 않습니다.** URL 인코딩되면 CSV에 박힌 주소를 사람이 읽을 수 없게 됩니다.

## 이미지 교체

**같은 파일명으로 덮어쓰면 CSV를 고칠 필요가 없습니다.** `raw.githubusercontent.com`은 `Cache-Control: max-age=300`이라 최대 5분 뒤 자동 반영됩니다. 바로 확인하려면 브라우저에서 하드 리프레시(`Ctrl+Shift+R`).

단, **가로세로 비율이 크게 달라지면 본문 레이아웃이 밀립니다.** 구도를 바꿀 때는 원래 비율을 비슷하게 맞추세요.

## 대조표

노션 `아마겟돈 / 챕터 내용 (2)` 데이터베이스에서 추출했습니다. 본문에 나오는 순서 그대로입니다.

> `chapter_id` 21(중립5 오답노트 활용 학습)과 26(안정5 퀴즈 시스템 활용 학습)은 삭제 예정이라 이미지가 없습니다.

### 기본 과정

| 파일명 | 노션 원본 | 들어갈 자리 |
|---|---|---|
| `ch1_01_trade_flow.png` | 픽셀아트_주식_거래_흐름_인포그래픽.png | 기본1 · 「주식의 기본 개념」 끝, 참고 상자 다음 |
| `ch1_02_delisting_timeline.png` | 상장폐지_절차_픽셀_타임라인.png | 기본1 · 「상장의 개념」 끝 |
| `ch1_03_dashboard.png` | 픽셀_스마트폰_주식_대시보드.png | 기본1 · 「시장 참여자 이해하기」 끝 |
| `ch2_01_trading_hours.png` | ChatGPT_이미지_2026년_10월_10일_오후_03_10_04.png | 기본2 · 「거래 시간과 방식」 끝 |
| `ch2_02_orderbook.png` | 레트로_픽셀_주식_호가창_스마트폰.png | 기본2 · 호가창 설명 뒤 |
| `ch2_03_market_vs_limit.png` | 시장가와_지정가_픽셀_안내서.png | 기본2 · 지정가 주문 설명 뒤 |
| `ch3_01_unrealized_vs_realized.png` | image.png | 기본3 · 평가손익·실현손익 설명 뒤 |
| `ch3_02_net_profit.png` | image.png | 기본3 · 순수익 계산 예시 뒤 |
| `ch4_01_market_cap.png` | image.png | 기본4 · 시가총액 설명 뒤 |
| `ch4_02_sectors.png` | image.png | 기본4 · 「업종의 이해」 끝 |
| `ch4_03_etf.png` | image.png | 기본4 · 「ETF 알아보기」 끝 |
| `ch5_01_index_weight.png` | img-n5-1.png | 기본5 · 이미지1. 시가총액이 큰 기업이 지수를 크게 움직이는 원리 |
| `ch5_02_business_cycle.png` | img-n5-2.png | 기본5 · 이미지2. 경기 순환 곡선 |
| `ch5_03_rate_bond.png` | img-n5-3.png | 기본5 · 이미지3. 금리와 채권 가격 시소 |
| `ch6_01_balance_sheet.png` | img-n6-1.png | 기본6 · 이미지1. 자산 = 자본 + 부채 구조 |
| `ch6_02_stock_split.png` | img-n6-2.png | 기본6 · 이미지2. 액면 분할 피자 비유 |
| `ch6_03_dividend_schedule.png` | img-n6-3.png | 기본6 · 이미지3. 배당 일정 |
| `ch7_01_candle.png` | image.png | 기본7 · 양봉·음봉 설명 뒤 |
| `ch7_02_moving_average.png` | image.png | 기본7 · 골든/데드 크로스 설명 뒤 |
| `ch7_03_technical_vs_value.png` | image.png | 기본7 · 「분석 방법의 이해」 끝 |
| `ch8_01_portfolio_weight.png` | image.png | 기본8 · 비중 관리 설명 뒤 |
| `ch8_02_volatility.png` | image.png | 기본8 · 「변동성 이해」 끝 |
| `ch8_03_investor_type.png` | image.png | 기본8 · 투자 성향 세 유형 뒤 |
| `ch8_04_split_trade.png` | image.png | 기본8 · 분할 매수·매도 설명 뒤 |
| `ch9_01_stoploss_takeprofit.png` | image.png | 기본9 · 이미지1. 익절선·손절선 |
| `ch9_02_averaging_down.png` | image.png | 기본9 · 이미지2. 물타기 |
| `ch9_03_loss_aversion.png` | image.png | 기본9 · 이미지3. 손실 회피 저울 |
| `ch10_01_vi.png` | image.png | 기본10 · 이미지1. VI 발동 흐름 |
| `ch10_02_circuit_breaker.png` | image.png | 기본10 · 이미지2. 서킷 브레이커 3단계 |
| `ch10_03_ipo.png` | image.png | 기본10 · 이미지3. 공모주 청약 ~ 상장일 |

### 공격형

| 파일명 | 노션 원본 | 들어갈 자리 |
|---|---|---|
| `ch11_01_box_range.png` | 픽셀_아트_돌파형_캔들_차트.png | 공격1 · 이미지1. 박스권 돌파 |
| `ch11_02_false_breakout.png` | 진짜_돌파와_속임수_돌파_비교.png | 공격1 · 이미지2. 진짜 돌파 / 속임수 돌파 |
| `ch11_03_risk_reward.png` | 픽셀_아트_매매_리스크보상_차트.png | 공격1 · 이미지3. 매수가·손절가·목표가 |
| `ch12_01_ratio_2to1.png` | 픽셀아트_2_1_보상_위험_차트.png | 공격2 · 이미지1. 손익비 2:1 막대 |
| `ch12_02_win_rate.png` | 5승_5패_순이익_50만.png | 공격2 · 이미지2. 5승 5패 누적 +50만 원 |
| `ch12_03_delayed_stoploss.png` | 원칙과_손절의_차이_PIXEL_차트.png | 공격2 · 이미지3. 손절을 미뤄 손익비가 뒤집히는 모습 |
| `ch13_01_sector_rotation.png` | 픽셀_아트_투자_순환_인포그래픽.png | 공격3 · 이미지1. 섹터 로테이션 |
| `ch13_02_golden_cross.png` | 민트_배경의_강세_돌파_차트.png | 공격3 · 이미지2. 5일선이 20일선을 돌파 |
| `ch14_01_rsi.png` | image.png | 공격4 · RSI 설명 뒤 |
| `ch14_02_volume_surge.png` | image.png | 공격4 · 「거래량 급증 패턴 분석」 뒤 |
| `ch14_03_limit_up.png` | image.png | 공격4 · 「상한가 연속성 전략」 끝 |
| `ch15_01_news_speed.png` | image.png | 공격5 · 「뉴스 이벤트 트레이딩의 개념」 끝 |
| `ch15_02_entry_rule.png` | image.png | 공격5 · 진입 절차 설명 뒤 |
| `ch16_01_win_rate_ratio.png` | image.png | 공격6 · 「모의투자 데이터의 중요성」 끝 |
| `ch16_02_loss_pattern.png` | image.png | 공격6 · 손실 패턴 분석 뒤 |
| `ch16_03_holding_period.png` | image.png | 공격6 · 「평균 보유기간 분석」 뒤 |

### 중립형

| 파일명 | 노션 원본 | 들어갈 자리 |
|---|---|---|
| `ch17_01_watchlist.png` | img-nut1-1.png | 중립1 · 이미지1. 관심 종목 리스트 화면 |
| `ch17_02_checklist.png` | img-nut1-2.png | 중립1 · 이미지2. 네 가지 체크리스트 |
| `ch17_03_entry_flow.png` | img-nut1-3.png | 중립1 · 이미지3. 진입 흐름 |
| `ch18_01_filter_funnel.png` | img-nut2-1.png | 중립2 · 이미지1. 2단계 필터 깔때기 |
| `ch18_02_real_vs_fake_breakout.png` | img-nut2-2.png | 중립2 · 이미지2. 진짜 돌파 / 가짜 돌파 |
| `ch18_03_entry_target_stop.png` | img-nut2-3.png | 중립2 · 이미지3. 매수가·목표가·손절가 |
| `ch19_01_bollinger.png` | img-nut3-1.png | 중립3 · 이미지1. 볼린저밴드 |
| `ch19_02_reduce_steps.png` | img-nut3-2.png | 중립3 · 이미지2. 비중 축소 단계 |
| `ch19_03_increase_steps.png` | img-nut3-3.png | 중립3 · 이미지3. 비중 확대 단계 |
| `ch20_01_three_way_buy.png` | image.png | 중립4 · 「3분할 매수 전략 실전」 뒤 |
| `ch20_02_rebalancing.png` | image.png | 중립4 · 리밸런싱 예시 뒤 |
| `ch20_03_sector_split.png` | image.png | 중립4 · 「업종 분산 실전 비율」 뒤 |
| `ch20_04_leverage_inverse.png` | image.png | 중립4 · 레버리지·인버스 ETF 설명 뒤 |

### 안정형

| 파일명 | 노션 원본 | 들어갈 자리 |
|---|---|---|
| `ch22_01_etf_basket.png` | image.png | 안정1 · 「ETF 중심 투자의 장점」 뒤 |
| `ch22_02_portfolio_ratio.png` | image.png | 안정1 · 「포트폴리오 구성 비율」 뒤 |
| `ch22_03_dca.png` | image.png | 안정1 · 정액 적립식 설명 뒤 |
| `ch22_04_rebalancing.png` | image.png | 안정1 · 「리밸런싱 전략」 뒤 |
| `ch23_01_dividend_growth.png` | image.png | 안정2 · 이미지1. 배당금 막대와 영업현금흐름 |
| `ch23_02_reinvest_compare.png` | image.png | 안정2 · 이미지2. 재투자 vs 현금 수령 비교 |
| `ch23_03_annual_review.png` | image.png | 안정2 · 이미지3. 5종목 균등 투자 + 연 1회 점검 |
| `ch24_01_alignment.png` | image.png | 안정3 · 이미지1. 정배열 상태에서 20% 조정 |
| `ch24_02_three_way_buy.png` | image.png | 안정3 · 이미지2. 3분할 매수와 평단가 |
| `ch24_03_target_stop.png` | image.png | 안정3 · 이미지3. 익절 목표선과 역배열 손절선 |
| `ch25_01_screening.png` | image.png | 안정4 · 이미지1. PBR·ROE 두 단계 스크리닝 |
| `ch25_02_dca.png` | image.png | 안정4 · 이미지2. 1~3월 주가와 매수 수량 |
| `ch25_03_rebalancing.png` | image.png | 안정4 · 이미지3. A 30%→20%, B 15%→20% 조정 |

---

노션 원본 파일명 중 `image.png`는 29장이 같은 이름이었습니다. 위 표의 "들어갈 자리"가 실제 구분 기준입니다.
