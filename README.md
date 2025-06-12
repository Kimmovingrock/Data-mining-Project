# 데이터 마이닝 프로젝트
미세먼지 중심의 의료 취약 지역 재정의
* LatLng
  * 행정구역시군구_경계
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
* WhoMergedPm
  * pm10 + pm25 전처리 후 생성
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
* hospital_per_area
  * 면적 당 병원 수
* hospital_per_pop
  * 인구 당 병원 수
* tmp_score_result
  * 기존 선행연구 바탕의 의료취약점수
