# 🎮 Phân tích dữ liệu doanh số game - Video Game Sales

Đây là đề tài cá nhân môn **Kho Dữ Liệu và Khai Phá Dữ Liệu**.  
Tập dữ liệu gồm hơn 16.000 tựa game với các thông tin: doanh số, thể loại, nền tảng, năm phát hành, nhà phát hành,...

---

## ✅ Mục tiêu:

- Trực quan hóa xu hướng phát hành & doanh số
- Dự đoán thể loại game từ doanh số
- Phân cụm nhóm game theo hành vi bán hàng

---

## 🚀 Hướng dẫn cài đặt & chạy

### 1. Clone repo:

```bash
git clone https://github.com/baolamabcd13/jupyter-khoa.git
cd jupyter-khoa
```

### 2. Tạo môi trường ảo:

```bash
python -m venv venv
# Windows:
venv\Scripts\activate
```

### 3. Cài đặt thư viện:

```bash
pip install -r requirements.txt
```

### 4. Chạy Jupyter Notebook:

```bash
jupyter notebook
```

---

## 📁 File chính

- `vgsales.ipynb`: toàn bộ quy trình phân tích và khai phá dữ liệu

---

## 📊 Các bước thực hiện

| PHẦN | Nội dung                                            |
| ---- | --------------------------------------------------- |
| 1️⃣   | Giới thiệu & Khảo sát dữ liệu                       |
| 2️⃣   | Thống kê thủ công + trực quan hóa                   |
| 2.5️⃣ | Min, Max, Mean, Median, Mode                        |
| 3️⃣   | Tương quan & PCA                                    |
| 3.1️⃣ | Cosine Similarity                                   |
| 4️⃣   | Phân cụm (DBSCAN + PCA)                             |
| 5️⃣   | Phân lớp dự đoán thể loại game (Decision Tree, KNN) |
| ⚔️   | So sánh mô hình + ROC Curve                         |
| 6️⃣   | Kết luận & đề xuất                                  |

---

## 🧪 Thư viện sử dụng

```txt
pandas
numpy
matplotlib
seaborn
scikit-learn
mlxtend
```

---

## 📚 Tài liệu tham khảo

- [https://www.kaggle.com](https://www.kaggle.com)
- [https://pandas.pydata.org](https://pandas.pydata.org)
- [https://scikit-learn.org](https://scikit-learn.org)

---

## 📝 DÀN Ý BÁO CÁO ĐỀ TÀI

### 1. Giới thiệu

- Mục tiêu phân tích & khai phá dữ liệu game
- Mô tả tập dữ liệu và nguồn gốc

### 2. Khảo sát & tiền xử lý

- Kiểm tra dữ liệu null, chuẩn hóa, mã hóa nhãn
- Sử dụng forward-fill để xử lý dữ liệu thiếu

### 3. Thống kê & trực quan

- Histogram, boxplot, barplot
- Thống kê: min, max, mean, median, mode

### 4. Tương quan & tương đồng

- Heatmap doanh số giữa các vùng
- Cosine similarity giữa các game

### 5. Khai phá dữ liệu

- PCA + DBSCAN: Phân cụm nhóm game
- Phân lớp `Genre` bằng Decision Tree & KNN
- So sánh mô hình bằng classification report & ROC

### 6. Kết luận & đề xuất

- Tóm tắt insight, mô hình tốt nhất
- Đề xuất mở rộng phân tích hoặc ứng dụng thực tiễn

---

## 📊 PHÂN TÍCH CÁC ĐỒ THỊ

| Biểu đồ                | Phân tích nhanh                          |
| ---------------------- | ---------------------------------------- |
| Countplot Year         | Game phát hành nhiều giai đoạn 2005–2010 |
| Histogram Global_Sales | Phần lớn game bán < 1 triệu bản          |
| Barplot Genre          | Action, Sports phổ biến nhất             |
| Heatmap Sales          | NA và EU tương quan mạnh                 |
| Cosine Similarity      | Game đầu tương đồng doanh số             |
| PCA scatter            | Dữ liệu phân nhóm rõ theo doanh số       |
| DBSCAN Clustering      | Phân cụm nhóm cao/trung/thấp             |
| ROC Curve              | KNN nhỉnh hơn DT về AUC                  |

---
