# 2374802010412
CÔNG NGHỆ SỬ DỤNG
1. PIL (Pillow): Đọc, chuyển đổi và lưu ảnh (Image.open(), convert())
2. Numpy: Xử lý mảng ảnh như ma trận (np.array, fft2, meshgrid)
3. Matplotlib: Hiển thị ảnh đầu vào / đầu ra(plt,imshow())
4. Scipy (fftpack) Thực hiện biến đổi Fourier nhanh 
5. Python cơ bản

GIẢI THÍCH CHI TIÊT TỪNG PHẦN 
1. Mờ ảnh và chuyển sang ảnh xám:
#Code: 
img = Image.open('bird.png').convert('L')
im_array = np.array(img)
#Giải thích
- Image.open() mở ảnh từ file
- .convert('L') chuyển ảnh sang grayscale
- np.array() chuyển ảnh thành ma trận số nguyên 2D(ảnh xám)

2. Fast Fourier Transform (FFT)
- fft2: biến đổi Fourier 2D ảnh 
- fftshift: Chuyển thành phố tần số với tâm ở giữa 
- log: tăng cường độ tương phản phổ
 3. Butterworth Lowpass Filter
 4. Butterworth Highpass Filter 

#Bài 1:
+ Công nghệ chính: Pillow + Numpy
+ Thuật toán nổi bật: Inverse, Gamma, Histogram 
+ Đặc điểm: tăng cường ảnh

#Bài 2: 
+ Công nghệ chính: FFT(SciPy)
+ Thuật toán nổi bật: FFT, Butterworth filters
+ Đặc điểm: tăng cường ảnh: Biến đổi miền tần số 

#Bài 3: 
+ Công nghệ chính: Ngẫu nhiên(Random) và những công nghệ trong bài 1
+ Thuật toán nổi bật: RGB shuffle + Random
+ Đặc điểm: tăng cường ảnh: Pha trộn auto

#Bài 4: 
+ Công nghệ chính: Ngẫu nhiên(Random) và những công nghệ có trong bài 2
+ Thuật toán nổi bật: RGB shuffle + Random Min/Max
+ Đặc điểm: tăng cường ảnh: Biến đổi Min Max
