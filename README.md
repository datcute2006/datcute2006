```
import random

def tung_xuc_xac():
 return [random.randint(1, 6) for _ in range(3)]

def tinh_diem(xuc_xac):
 return sum(xuc_xac)

def kiem_tra_ket_qua(diem):
 if diem >= 10 and diem <= 17:
 return "Tài"
 elif diem >= 4 and diem <= 9:
 return "Xỉu"
 else:
 return "Cửa khác"

def tro_choi():
 print("Tài Xỉu")
 print("---------")
 cược = input("Đặt cược (Tài/Xỉu/Cửa khác): ")
 xuc_xac = tung_xuc_xac()
 diem = tinh_diem(xuc_xac)
 ket_qua = kiem_tra_ket_qua(diem)
 print(f"Xúc xắc: {xuc_xac}")
 print(f"Điểm: {diem}")
 print(f"Kết quả: {ket_qua}")
 if ket_qua == cược:
 print("Chúc mừng! Bạn thắng!")
 else:
 print("Better luck next time!")

tro_choi()
```
