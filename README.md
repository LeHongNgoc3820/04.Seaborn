# Trực quan hoá dữ liệu với Seaborn
[**Chi tiết bài viết**](  )

**Dưới đây là tóm tắt lí thuyết**

## 1. Giới thiệu Seaborn
+ Với Analytics, cách tốt nhất để có được thông tin chi tiết là bằng cách trực quan hoá dữ liệu. Dữ liệu có thể được hình dung bằng cách biểu diễn như là các ô dễ hiểu, dễ khám phá và nắm bắt. Dữ liệu này giúp thu hút sự chú ý của các yếu tố chính.
+ Để phân tích một tập hợp dữ liệu bằng Python, có thể sử dụng Matplotlib, một thư viện 2D được triển khai rộng rãi hoặc **Seaborn** (là một thư viện trực quan bằng Python, được xây dựng trên Matplotlib).

### 1.1 Đặc điểm của Seaborn
+ Seaborn được xây dựng trên thư viện trực quan cốt lõi của Python là Matplotlib. **Seaborn là một phần bổ sung và không phải là một sự thay thế cho Matplotlib.**
+ Tuy nhiên, Seaborn có một số tính năng rất quan trọng như:
    + Trực quan hoá dữ liệu đơn biến và hai biến
    + Phù hợp và hình dung các mô hình hồi quy tuyến tính
    + Lập kế hoạch dữ liệu chuỗi thời gian thống kê
    + Seaborn hoạt động tốt với cấu trúc dữ liệu NumPy và Pandas
    + Nó đi kèm với các theme để tạo kiểu Matplotlib đồ hoạ
    
### 1.2 So sánh Seaborn với Matplotlib
+ Matplotlib "cố gắng làm mọi việc dễ dàng hơn và làm cho việc khó khăn có thể giải quyết". Seaborn hỗ trợ các phương pháp trực quan hoá dữ liệu phức tạp hơn nhưng vẫn cần Matplotlib.
+ Seaborn giúp giải quyết vấn đề lớn mà Matplotlib phải đối mặt, đó là:
    + Các tham số Matplotlib mặc định (Seaborn hoạt động với các tham số tuỳ chỉnh khác nhau)
    + Matplotlib làm việc với DataFrame không suôn sẻ, chỉ làm việc với các cột dữ liệu cụ thể trên DataFrame còn ngược lại, Seaborn làm việc với DataFrame  và array chứa toàn bộ dữ liệu)

### 1.3 Cài đặt Seaborn
**Sử dụng:** `pip intstall seaborn`

**Import thư viện:**

`import seaborn as sns` hoặc `import seaborn as sb`

## 2. Các biểu đồ thường dùng trong Seaborn

Các dạng biểu đồ được chia theo 4 nhóm như sau:

**a. Frequency Distribution - Categorical Variables**
+ countplot 
+ catplot

**b. Distribution of the Numerical Variable**
+ distplot(histogram)
+ kdeplot
+ boxplot
+ violinplot

**c. Relationship between 2 Numerical Variables**
+ lineplot
+ scatterplot
+ relplot
+ jointplot
+ lmplot
+ heatmap
+ pairplot
+ facetgrid

**d. Relationship between Numerical and Categorical Variables**
+ pointplot
+ barplot
+ boxplot
+ violinplot
+ swarmplot


## 3. Tổng kết
### Một số lưu ý khi lựa chọn biểu đồ:
**Phân tích phân phối đơn biến (Univariate Distribution Analysis)**
+ Tốt nhất nên dùng `distplot()`
+ Phương án thay thế: `rugplot()` hoặc `kdeplot()`

**Phân tích hồi quy**
+ Dùng `lmplot()`, `regplot()`
+ Note: `plt.scatter()` của Matplotlib

**Biểu đồ phân loại**
+ `factorplot()`
+ `barplot()`, `pointplot()`, `countplot()`
+ `boxplot()`, `violinplot()`
+ `swarmplot()`
