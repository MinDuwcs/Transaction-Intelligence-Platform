# AI Financial Intelligence Risk Analytics Platform
Nền tảng sử dụng Data Pipeline + AI xử lý dữ liệu tài chính bán thực tế: giao dịch, hóa đơn, sao kê, ticket hỗ trợ khách hàng. Hệ thống sẽ ingest dữ liệu, làm sạch, lưu vào database, chạy phân tích rủi ro, dùng AI để truy vấn, giải thích bất thường, và hiển thị dashboard.

## Mô tả
Xây dựng hệ thống phân tích giao dịch tài chính để phát hiện các giao dịch có rủi ro cao hoặc bất thường, sau đó hiển thị kết quả lên dashboard và cung cấp giải thích bằng AI.

## Mục Tiêu Dự Án
Xây dựng một hệ thống có khả năng:
  - Thu thập dữ liệu tài chính, tin tức hoặc dữ liệu giao dịch mẫu.
  - Làm sạch, xử lý, chuẩn hóa và lưu vào database.
  - Tạo pipeline ETL/ELT có thể chạy định kỳ.
  - Xây API backend để truy xuất dữ liệu và kết quả AI.
  - Xây model AI hoặc module AI để phân tích rủi ro, phân loại bất thường, tóm tắt insight.
  - Xây dashboard frontend để người dùng xem dữ liệu, cảnh báo, biểu đồ và phân tích.
  - Đóng gói bằng Docker và deploy bản demo.

## Tính Năng Chính Ver 1.0
  - Ingest dữ liệu tài chính hoặc dữ liệu giao dịch mẫu.
  - Lưu vào PostgreSQL.
  - Xây pipeline xử lý dữ liệu bằng Python.
  - Xây API bằng FastAPI.
  - Xây dashboard bằng React/Next.js.
  - Tích hợp module AI:
    - phát hiện giao dịch bất thường, hoặc
    - phân loại rủi ro, hoặc
    - tóm tắt insight bằng LLM.
  - Docker Compose để chạy toàn bộ hệ thống.
  - Deploy bản demo.
## Tính Năng Bổ Sung Ver 2.0 (Nếu đủ thời gian)
  - Data orchestration bằng Airflow hoặc Prefect.
  - Vector database cho semantic search.
  - LangChain/LangGraph cho AI workflow.
  - Model tracking bằng MLflow.
  - Authentication đơn giản.
  - Monitoring/logging.
  - CI/CD bằng GitHub Actions.

## Thiết Kế Kiến Trúc Hệ Thống
````
Data Sources
    |
    v
Data Ingestion Pipeline
    |
    v
Data Processing / Feature Engineering
    |
    v
Database / Data Warehouse
    |
    v
ML / AI Models
    |
    v
Backend API
    |
    v
Frontend Dashboard
````
## Nguồn Dữ Liệu Được Sử Dụng
| Bộ Dữ Liệu                           | Mô Tả                                                                           | Link                           |
| ------------------------------------ | --------------------------------------------------------------------------------| ------------------------------ |
| Synthetic Banking Dataset            | Bộ dữ liệu này là một mô phỏng cơ sở dữ liệu ngân hàng tổng hợp quy mô lớn      | [Source](https://www.kaggle.com/datasets/akrambelha/synthetic-banking-dataset-csv-sql-sqlite)              |
| Credit Card Fraud Detection          | Dữ liệu này chứa các giao dịch được thực hiện bằng thẻ tín dụng đã được bảo mật | [Source](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)               |
| SEC EDGAR Company Fundamentals (API) | Hệ thống công khai báo cáo tài chính của các công ty niêm yết tại Mỹ            | [Source]()               |

## Công Nghệ Sử Dụng
| Layer           | Công nghệ                        | Vai trò                        |
| --------------- | -------------------------------- | ------------------------------ |
| Language        | Python                           | ETL, AI, backend               |
| Backend         | FastAPI                          | REST API                       |
| Database        | PostgreSQL                       | Lưu dữ liệu có cấu trúc        |
| Frontend        | Streamlit (Version 1)            | Dashboard demo                 |
| Container       | Docker, Docker Compose           | Chạy toàn bộ hệ thống          |
| AI/ML           | scikit-learn, PyTorch tùy mức độ | Model phân tích rủi ro/anomaly |
| LLM Workflow    | LangChain hoặc LangGraph         | Tóm tắt insight, Q&A dữ liệu   |
| Notebook        | Jupyter/Colab                    | Experiment ban đầu             |
| Version Control | Git, GitHub                      | Portfolio repo                 |

## Hướng Dẫn Cài Đặt

## Ví Dụ Sử Dụng

## Cấu Trúc Thư Mục Dự Kiến
```
├── backend/
│   ├── app/
│   │   ├── api/
│   │   ├── core/
│   │   ├── models/
│   │   ├── services/
│   │   └── main.py
│   ├── tests/
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── external/
│
├── notebooks/
│
├── scripts/
│   ├── run_pipeline.py
│   └── train_model.py
│
├── models/
│
├── docs/
│
├── docker/
│
├── .env.example
├── .gitignore
├── docker-compose.yml
├── README.md
└── LICENSE
```
## Phụ Thuộc
**Backed:**
  - fastapi
  - uvicorn
  - pandas
  - numpy
  - scikit-learn
  - sqlalchemy
  - psycopg2-binary
  - pydantic
  - python-dotenv

**Machine Learning / AI:**
  - Pytorch
  - scikit-learn
  - langchain
  - langgraph
  - sentence-transformers
  - faiss-cpu

**Frontend:**
  - react
  - next
  - typescript
  - tailwindcss
  - axios
  - recharts

**Database / Infrastructure:**
  - postgresql
  - docker
  - docker-compose






























