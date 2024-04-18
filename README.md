# spstats

과제 제출용
동아대학교 2342709 김강민

패키지 링크 : https://pypi.org/project/spstats/

깃허브 레퍼지토리 : https://github.com/VERUS2621/statis0001

다운로드 : pip install spstats

사용방법 : from spstats import spstats as sp


저는 확률과 통계 수업에서 numpy, pandas, scipy, matplotlib.pyplot 모듈을 사용하는 것을 보고 4가지를 한 번에 합치면 편하겠다는 생각이 들어 합치게 되었습니다.
밑에 작성되지 않은 함수는 sp.np ~, sp.pd ~ 등으로 사용하면 되겠습니다.

이`spstats` 라이브러리의 각 함수를 간단히 설명하여 정리해 보겠습니다.

from spstats import spstats as sp

- example
data = sp.array([1,2,3,4,5,5,5,5,6,6,7,8,8])

print(len(data))

print(sp.mean(data))

print(sp.med(data))

print(sp.std(data))

print(sp.var(data))


13 

5.0

5.0

2.0380986614602725

4.153846153846154



1. `randomarr(size):`
    - 지정된 크기의 랜덤한 NumPy 배열을 생성합니다.

2. `array(data):`
    - Numpy 배열을 선언합니다.

3. `mean(data):`
    - NumPy 배열 또는 Pandas Series의 평균을 계산합니다.

4. `mode(data):`
    - NumPy 배열 또는 Pandas Series의 최빈값을 계산합니다. // 인덱스 오류가 있어 현재는 수정하였으나 지금 작동하지 않음

5. `med(data):`
    - NumPy 배열 또는 Pandas Series의 중앙값을 계산합니다.

6. `std(data):`
    - NumPy 배열 또는 Pandas Series의 표준편차를 계산합니다.

7. `var(data):`
    - NumPy 배열 또는 Pandas Series의 분산을 계산합니다.

8. `skew(data):`
    - 데이터의 왜도를 계산합니다.

9. `kurtosis(data):`
    - 데이터의 첨도를 계산합니다.

10. `hist(data, xlabel, ylabel, title):`
    - NumPy 배열 또는 Pandas Series의 히스토그램을 플로팅합니다. 데이터의 길이를 기반으로 bin의 수를 결정합니다.

11. `pie(data, labels, title):`
    - 파이 차트를 생성합니다.

12. `line_plot(x, y, xlabel, ylabel, title):`
    - 두 데이터 집합의 선 그래프를 생성합니다.

13. `scatter_plot(x, y, xlabel, ylabel, title):`
    - 두 데이터 집합의 산점도를 생성합니다.

14. `bar(categories, values, xlabel, ylabel, title):`
    - 막대 그래프를 생성합니다.

15. `savefig(filename):`
    - 그림을 저장합니다.

16. `t_test(data1, data2):`
    - scipy.stats를 사용하여 두 샘플에 대한 t-test을 수행합니다.

17. `correlation(data1, data2):`
    - 두 데이터 집합 사이의 피어슨 상관 계수를 계산합니다.

18. `standardize(data):`
    - 데이터 집합의 값을 표준화합니다.

19. `box_plot(data, xlabel, ylabel, title):`
    - 데이터 집합의 상자 그림을 생성합니다.

20. `linear_regression(x, y):`
    - 두 데이터 집합에 대한 선형 회귀를 수행합니다.

21. `bootstrap_resample(data, n_samples):`
    - 데이터 집합에 대한 부트스트랩 재 표본을 생성합니다.

22. `probability_distribution(rv, size=1000):`
    - 주어진 무작위 변수를 기반으로 확률분포표를 작성합니다.

23. `describe(data):`
    - NumPy 배열 또는 Pandas의 describe를 반환합니다.
