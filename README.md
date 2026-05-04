# AutoMobile-Midterm

자율이동체시스템 중간고사 대체 과제 (2026, 성신여자대학교)

## 📋 과제 개요

KITTI Odometry 데이터셋의 **Sequence 09**를 이용하여:
1. Bayesian 기반 도로 영역 분류
2. Projection Matrix 해석 및 활용
3. 차량 궤적 시각화
4. 차선 검출 및 실패 구간 분석
5. 딥러닝 모델 비교

## 📁 프로젝트 구조

```
AutoMobile-Midterm/
├── auto_class_2_BayesianClassifier.ipynb   # 과제 제출 메인 노트북
├── README.md
├── .gitignore
└── results/                                  # 분류 결과 (대표 샘플만 포함)
    └── bayes_road_09/
        ├── overlay_*.png
        └── road_ratios.csv
```

> ⚠️ `dataset/` 폴더는 KITTI 데이터셋이며, 용량 문제로 git에 포함되지 않습니다.
> KITTI Odometry 데이터셋(Sequence 09)을 별도로 다운로드하여 다음 위치에 배치해야 합니다:
> - `dataset/sequences/09/image_0/`
> - `dataset/sequences/09/calib.txt`
> - `dataset/sequences/09/times.txt`
> - `dataset/poses/09.txt`

## 🛠️ 실행 환경

- Python 3.10+
- numpy, pandas, matplotlib, opencv-python, pillow, scikit-learn

```bash
pip install numpy pandas matplotlib opencv-python pillow scikit-learn jupyter
```

## 📚 참고 자료

- 수업 자료: [yangjunahn/ClassAuto/auto_class_1_camera.ipynb](https://github.com/yangjunahn/ClassAuto/blob/main/auto_class_1_camera.ipynb)
- 베이스 코드: [yangjunahn/ClassAuto/auto_class_2_BayesianClassifier.ipynb](https://github.com/yangjunahn/ClassAuto/blob/main/auto_class_2_BayesianClassifier.ipynb)
- OpenCV calib3d: https://docs.opencv.org/4.x/d9/d0c/group__calib3d.html
- KITTI Odometry: https://www.cvlibs.net/datasets/kitti/eval_odometry.php
