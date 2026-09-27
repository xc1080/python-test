# Python Calculator Tests

[![Python](https://img.shields.io/badge/Python-3.11-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![pytest](https://img.shields.io/badge/tested%20with-pytest-0A9EDC?logo=pytest&logoColor=white)](https://pytest.org/)
[![CI](https://img.shields.io/badge/CI-GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)](https://github.com/features/actions)

一个用于学习 Python 单元测试与 GitHub Actions 的小型示例项目，提供加法、乘法函数以及对应的 pytest 测试。

## 运行测试

```bash
python -m pip install pytest
pytest -v
```

每次 push 或 pull request 都会触发 `.github/workflows/ci.yml` 中的自动测试。

## 文件说明

```text
├── calculator.py       # add 与 multiply 函数
├── test_calculator.py  # pytest 测试用例
└── .github/workflows/  # GitHub Actions 配置
```

> 注意：仓库当前的 `requirements.txt` 是二进制文件，并非有效的 pip 依赖清单，因此本项目直接通过命令安装 `pytest`。

