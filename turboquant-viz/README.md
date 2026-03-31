# TurboQuant Rotation Study

TurboQuant(arXiv 2504.19874)의 랜덤 직교행렬 R을 FWHT(Fast Walsh-Hadamard Transform)로 대체할 수 있는지 검증하는 interactive visualization.

## Live Demo

**https://junhyeongkim-kr.github.io/turboquant-viz/**

## Visualizations

| Page | Description |
|------|-------------|
| [rotation_compare_2d](rotation_compare_2d.html) | 2D에서 R vs HD 단계별 벡터 변환 비교 |
| [r_vs_fwht_by_dimension](r_vs_fwht_by_dimension.html) | d=2~256 차원별 R vs FWHT 출력 분포 scatter + histogram |
| [cascade_hd_deploy](cascade_hd_deploy.html) | HD 1~4회 반복(cascade) 시 분포 변화, D 고정 |
| [qjl_matrix_compare](qjl_matrix_compare.html) | QJL 행렬: N(0,1) vs SRHT vs Rademacher 비교 |

## Key Findings

- **d >= 64**: HD 1회만으로 R과 구별 불가능
- **d < 16**: cascade HD 2~3회 적용으로 개선 가능
- **QJL**: SRHT(O(d log d))와 Rademacher(O(d^2) 빠른 상수)로 대체 가능

## Usage

외부 의존성 없음. HTML 파일을 브라우저에서 직접 열면 동작합니다.
