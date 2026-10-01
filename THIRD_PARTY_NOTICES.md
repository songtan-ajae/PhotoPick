# 외부 구성요소와 저작권 고지

PhotoPick 공개 저장소는 실행파일 배포 전용입니다. 자체 구현 소스코드는 공개하지 않으며 앱 전체에 MIT 등 오픈소스 라이선스를 부여하지 않습니다. 아래의 라이선스는 **각 외부 구성요소**에 적용됩니다.

| 구성요소 | 원 출처 | 포함된 고지 |
| --- | --- | --- |
| Flutter framework | [flutter/flutter](https://github.com/flutter/flutter/blob/master/LICENSE) | `licenses/Flutter-LICENSE.txt` · BSD-3-Clause |
| Dart | [dart-lang/sdk](https://github.com/dart-lang/sdk) | `licenses/Dart-LICENSE.txt` · BSD-3-Clause |
| Flutter engine 및 외부 엔진 구성요소 | 빌드 SDK의 sky_engine 라이선스 집계 | `licenses/Flutter-Engine-THIRD-PARTY-LICENSES.txt` |
| Dart/Flutter 패키지 | 검증된 앱 빌드의 생성된 집계 | 실행 패키지의 `data/flutter_assets/NOTICES.Z` 및 `licenses/Flutter-Packages-NOTICES.txt` |
| ONNX Runtime 1.22.0 | [microsoft/onnxruntime](https://github.com/microsoft/onnxruntime) | `licenses/ONNX-Runtime-LICENSE.txt` · MIT, `licenses/ONNX-Runtime-ThirdPartyNotices.txt` |
| flutter_onnxruntime | MASIC AI | `licenses/flutter_onnxruntime-LICENSE.txt` · MIT |
| NIMA MobileNet 기술 품질 모델 | [idealo/image-quality-assessment](https://github.com/idealo/image-quality-assessment), [ONNX 변환본 배포처](https://huggingface.co/hugglyberry/upscale-and-refine-models/blob/main/nima-mobilenet-quality.onnx) | `licenses/LICENSE-NIMA.txt` · 원 프로젝트 Apache-2.0 |
| Pretendard 1.3.9 | [orioncactus/pretendard](https://github.com/orioncactus/pretendard) | `licenses/OFL-Pretendard.txt` · SIL OFL 1.1 |
| Cupertino Icons | 패키지 배포본 | `licenses/Cupertino-Icons-LICENSE.txt` · MIT |
| Material Icons | [google/material-design-icons](https://github.com/google/material-design-icons) | `licenses/Material-Icons-LICENSE.txt` · Apache-2.0 |
| 오프라인 설명용 사진 네 장 | Jakub Hałun / Wikimedia Commons | `licenses/EXAMPLE-PHOTOS-CREDITS.md` · CC BY 4.0 |
| README 캡처 속 사진 | Jakub Hałun / Wikimedia Commons | [캡처 출처](docs/SCREENSHOTS.md) · CC BY 4.0 |

## 변경 및 모델 출처

`flutter_onnxruntime` Windows 플러그인에는 UI 스레드 밖에서 추론하도록 로컬 수정이 있습니다. 원 MIT 저작권 고지는 유지했습니다.

배포한 NIMA ONNX 파일은 기존 변환본 그대로이며 이번 공개 패키징에서 가중치를 수정하거나 재학습하지 않았습니다. PhotoPick은 추론 출력에 자체 로컬 품질 검사와 취향 특성을 결합합니다. 모델 SHA-256은 `D79D3417FD046099E452DE39DA3FC18334E0EF5A4E4E3CB62782232420E66748`입니다.

변환본 저장소는 모델별 원 프로젝트 라이선스를 유지하는 혼합 라이선스 저장소입니다. 그 요약에는 NIMA가 MIT로 적혀 있으나, 연결된 idealo 원 프로젝트의 실제 LICENSE는 Apache-2.0이므로 이 배포에서는 원 Apache-2.0 전문과 저작권을 포함했습니다. 원 TID2013/AVA 학습 데이터셋은 이 배포에 포함하지 않습니다.

설명용 예시 사진은 화면에서 흐림·밝기·대비 변화를 시연할 수 있습니다. 원 사진 저작권, 변경 안내, 라이선스 링크를 별도 고지에 유지했습니다. 저작권 표기는 사진·모델·폰트를 PhotoPick 자체 저작물로 주장하지 않습니다.

## 배포 구성

실행 ZIP에는 실행파일, 런타임 DLL, 모델, 폰트, 설명 자산, 사용자 안내, 원 라이선스 전문이 포함됩니다. 사용자 사진 모음, 분류/취향 프로필, 개발 로그, 검증 원본 보고서, 앱 구현 소스는 포함하지 않습니다.

각 원문과 적용 조건은 개별 고지 파일을 확인하세요. 이 표는 구성요소 출처 안내이며 별도의 법률 자문이나 Google/Microsoft 등 원 저작자의 제품 인증을 의미하지 않습니다.
