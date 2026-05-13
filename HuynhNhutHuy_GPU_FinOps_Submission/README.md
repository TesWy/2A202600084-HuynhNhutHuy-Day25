# Bài nộp GPU FinOps - Huynh Nhut Huy

Sinh viên: Huynh Nhut Huy  
MSSV: 2A202600084

## Nội dung bài nộp

- `notebook/gpu_finops_lab.ipynb`: notebook Kaggle đã chạy và lưu output đến Cell 31.
- `generated_charts/`: 9 biểu đồ PNG được sinh ra từ notebook.
- `screenshots/`: ảnh chụp/evidence cho toàn bộ các phần yêu cầu trong bài.

## Tóm tắt kết quả

- Notebook đã chạy đầy đủ các phần từ Part 1 đến Part 8.5.
- Kaggle notebook đã bật GPU và Internet.
- Real GPU workload đã chạy trên Tesla T4, bao gồm:
  - detect GPU thật;
  - thu thập GPU telemetry;
  - train FP32 baseline;
  - train Mixed Precision AMP;
  - so sánh thời gian, chi phí và mức tiết kiệm;
  - report chi phí về FinOps gateway.
- Part 8.5 đã hoàn thành phần advanced analysis:
  - multi-GPU cost analysis cho cấu hình 1, 2, 4 và 8 GPU;
  - project cost forecasting;
  - optimization opportunity analysis;
  - integrated cost dashboard;
  - challenge optimization strategy.

## Evidence quan trọng

- `screenshots/kaggle_gpu_t4x2_runtime.png`: ảnh chụp Kaggle Session options cho thấy accelerator đang chọn `GPU T4 x2`.
- `screenshots/part8_gpu_detection.png`: output detect GPU thật trong notebook.
- `screenshots/part8_fp32_summary.png`: kết quả train FP32.
- `screenshots/part8_amp_summary.png`: kết quả train AMP.
- `screenshots/part8_fp32_vs_amp_comparison.png`: so sánh FP32 và AMP.
- `screenshots/part8_real_gpu_cost_report.png`: cost report gửi về gateway.
- `screenshots/part85_multi_gpu_analysis.png`: phân tích chi phí/scaling multi-GPU.
- `screenshots/part85_integrated_dashboard.png`: dashboard tổng hợp advanced FinOps.
- `screenshots/part85_challenge_strategy.png`: chiến lược tối ưu chi phí cho challenge.

## Ghi chú về yêu cầu 2 GPU

Ảnh `kaggle_gpu_t4x2_runtime.png` chứng minh runtime Kaggle đã được cấu hình với `GPU T4 x2`. Trong notebook, phần real training chạy workload thực tế trên GPU, còn phần Part 8.5 phân tích chi phí và hiệu quả scaling cho nhiều cấu hình GPU, bao gồm 2 GPU. Theo checklist trong `SUBMISSION.md`, yêu cầu chính là bật GPU trên Kaggle/Colab, chạy real GPU workload và hoàn thành multi-GPU cost analysis.

## Trạng thái hoàn thành

- Đủ notebook đã chạy output.
- Đủ ảnh evidence cho các phần yêu cầu.
- Đủ 9 biểu đồ sinh ra từ notebook.
- Có thêm ảnh xác nhận Kaggle runtime dùng `GPU T4 x2`.
