### praktikum4

## Soal praktikum4



![1.png](/gambar4/1.png)


![2.png](/gambar4/2.png)

Hasil ouput pada praktikum4

![3.png](/gambar4/3.png)




### code untuk latihan pratikum 4

		# -*- coding: utf-8 -*-
			"""
		Spyder Editor

		This is a temporary script file.
			"""

			n = 0
			nm = []
			nim = []
			tugas = []
			uts = []
			uas = []
			akhir = []

			while True:
    				Nama = input("Nama      :")
    				nm.append(Nama)
    				Nim = input("NIM       :")
    				nim.append(Nim)
    				Tugas = input("Tugas      :")
    				tugas.append(Tugas)
    				Uts = input("UTS       :")
    				uts.append(Uts)
    				Uas = input("UAS       :")
    				uas.append(Uas)
    				Akhir = (int(Tugas)* .30) + (int(Uts)* .35) + (int(Uas)* .35)
    				akhir.append(Akhir)
    
    				data = ' '
    				while data != 'Y' and data != 'T':
        				data = input("Tambah data [Y/T] ?")
        
    				n += 1
    				if data == 'T':
        				break
    
			print("=================================================================")
			print("NO   |   NAMA   |   NIM    |  TUGAS   | UTS   |  UAS  |   AKHIR ")
			print("=================================================================")
    
			for a in range(n):
    				print("",a+1, "|" ,nm[a],"      |" , nim[a], "|", tugas[a], "|", uts[a], "|", 
          			uas[a], "|", akhir[a], "|")


### praktikum5

## soal praktikum5



![1.png](/gambar5/1.png)

![2.png](/gambar5/2.png)

Hasil ouput pada praktikum5

![3.png](/gambar5/3.png)

![4.png](/gambar5/4.png)



### code untuk latihan praktikum 5

		# -*- coding: utf-8 -*-
		"""
		Created on Wed Nov 25 15:48:46 2020

		@author: ASUS
		"""

		print("======================================================================")
		print("=========================> Program Input Data <=======================")
		print("======================================================================")
		data = {}
		while True:
    			print("")
    			m = input("===>> (L)ihat,  (T)ambah,  (U)bah,  (H)apus,  (C)ari,  (K)eluar <<=== : ")
    			print("========================================================================")
    			print("| NO |     Nama      |     Nim     |  Tugas  |  UTS  |  UAS  |  Akhir  |")
    			print("========================================================================")
    			print(">>>>>>>>>>>>>>>>>>>>>>>> TIDAK ADA DATA <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<")
    			if m.lower() == 'k' :
        			break
    
    			elif m.lower() == 'l' :
        			print("DAFTAR NILAI")
        			print("=====================================================================")
        			print("| NO |     NAMA    |    NIM     |  TUGAS  |  UTS  |  UAS  |  AKHIR  |")
        			print("=====================================================================")
        			i = 0
        			for x in data.items():
            				i += 1
            				print(" 1 |  {0:9}  |  {1:9}  |  {2:9}  |  {3:9}  |  {4:9}  |  {5:9}  |" .format(
                				x[0], x[1][0], x[1][1], x[1][2], x[1][3], x[1][4]))
            
  			      	else:
            				print("Tidak ada Data")
        
    			elif m.lower() == 't' :
        			print("Tambah Data")
        			nama = input("Nama                        : ")
        			nim = input("Nim                          : ")
        			tugas = float(input("Masukan Nilai Tugas  : "))
       				uts = float(input("Masukan Nilai UTS      : "))
        			uas = float(input("Masukan Nilai UAS      : "))
        			akhir = (0.30 * tugas) + (0.35 * uts) + (0.35 * uas)
        			data[nama] = nim, tugas, uts, uas, akhir
        
    			elif m.lower() == 'u' :
        			print("Ubah Data Mahasiswa")
        			nama = input("Nama  : ")
        			if nama in data.keys():
            				nim = input("Nim  :")
            				tugas = float(input("Masukan Nilai tugas : " ))
            				uts = float(input("Masukan Nilai uts  : "))
            				uas = float(input("Masukan Nilai uas  : "))
            				akhir = (0.30 * tugas) + (0.35 * uts) + (0.35 * uas)
            				data[nama] = nim, tugas, uts, uas, akhir
        
        			else:
            				print("Tidak ada Data")
    
    			elif m.lower() == 'h' :
        			print("Hapus Data Mahasiswa")
        			nama = input("Nama   : ")
        			if nama in data.keys():
            				print("Datanya", nama, "adalah {0}".format(data[nama]))
        			else:
            				print("Tidak ada Data")
    
    			else:
        			print("Plih menu yang tersedia")

