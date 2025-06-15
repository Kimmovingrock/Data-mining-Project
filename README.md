# 데이터 마이닝 프로젝트
미세먼지 중심의 의료 취약 지역 재정의
* LatLng
  * 행정구역시군구_경계 (파일이 커서 직접 다운로드 후 사용해야 합니다.
  * https://drive.google.com/drive/folders/1N-fPoLz3qM2ozBbYCdtk6FhaCt4RX1iM?usp=drive_link
  * 출처 : https://www.data.go.kr/data/15125045/fileData.do?recommendDataYn=Y#
* hazard_facility
  * 시군구 단위 대기 배출원
  * 출처 : https://www.data.go.kr/data/15068820/fileData.do
* pm10.csv
  * pm10 미세먼지 데이터
  * 출처: https://kosis.kr/statHtml/statHtml.do?sso=ok&returnurl=https%3A%2F%2Fkosis.kr%3A443%2FstatHtml%2FstatHtml.do%3FtblId%3DDT_106N_03_0200045%26orgId%3D106%26
* pm25.csv
  * pm2.5 미세먼지 데이터
  * 출처: https://kosis.kr/statHtml/statHtml.do?sso=ok&returnurl=https%3A%2F%2Fkosis.kr%3A443%2FstatHtml%2FstatHtml.do%3Fconn_path%3DI3%26tblId%3DDT_106N_03_0200145%26orgId%3D106%26
* population.csv
  * 지역별 인구수
  * 출처 : https://kosis.kr/statHtml/statHtml.do?sso=ok&returnurl=https%3A%2F%2Fkosis.kr%3A443%2FstatHtml%2FstatHtml.do%3FtblId%3DDT_1B040A3%26orgId%3D101%26
* hospital.xlsx
  * 지역별 병원 수 -> hospital_compined.csv(각 필드 병합) -> hospital_cleaned.csv
  * 출처 : https://opendata.hira.or.kr/op/opc/olapYadmStatInfoTab2.do
* area.csv
  * 지역별 면적
  * 출처 : https://kosis.kr/statHtml/statHtml.do?sso=ok&returnurl=https%3A%2F%2Fkosis.kr%3A443%2FstatHtml%2FstatHtml.do%3Fconn_path%3DI2%26tblId%3DDT_1YL21291E%26orgId%3D101%26
* elderly_pop.csv
  * 고령인구비율 데이터
  * https://kosis.kr/statHtml/statHtml.do?sso=ok&returnurl=https%3A%2F%2Fkosis.kr%3A443%2FstatHtml%2FstatHtml.do%3Fconn_path%3DI2%26tblId%3DDT_1YL20631%26orgId%3D101%26
* outpatient, patient(atopic)
  * 아토피 왜래, 내원환자 데이터
  * https://www.data.go.kr/data/15104805/fileData.do
* outpatient, patient(rhinitis)
  * 비염 왜래, 내원환자 데이터
  * https://www.data.go.kr/data/15104804/fileData.do?recommendDataYn=Y
* outpatient, patient(asthma) / city_county_code
  * 천식 외래, 내원환자 데이터, 시군구 코드 데이터
  * https://www.data.go.kr/data/15104806/fileData.do?recommendDataYn=Y


* progressing_score.ipynb(1번째로 실행)
  * pm2.5, pm10 데이터 전처리 및 병합
  * 병원 수, 지역 면적, 인구 수, 고령인구 비율을 전처리하여 tmp_score.scv 도출 후 main.ipynb에서 사용
* respiratory_case.ipynb(2번째로 실행)
  * patient, outpatient(asthma) / patient, outpatient(atopic) / patient, outpatient(rhinitis) + city_county_code 천식, 아토피, 비염 각 외래, 내원 환자수 전처리 + 시군구 데이터 병합
* main.ipynb (3번째로 실행)
  * 유해시설 점수 평가
  * 클러스터링을 통한 미세먼지 중심 의료취약지역 선정
  * 자료 시각화
  * XGBoost 모델 학습
 
* 실행 및 테스트 환경
  * python 3.11.9, 3.12.7
  * 추가 install
  * pip install folium
  * pip install geopandas
  * pip install numpy
  * pip install pandas
  * pip install xgboost
  * pip install openpyxl
  * pip install scikit-learn
  * pip install matplotlib
