# tugas-dasar-pemerograman-pertemuan-3

{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "NAMA : Rio Luigi Del Niery\n",
    "\n",
    "NIM : 20220040120\n",
    "\n",
    "KELAS : TI22J"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "#SOAL NO 1\n",
    "1. Operator Aritmatika\n",
    "digunakan dengan nilai numerik untuk melakukan operasi \n",
    "matematika umum.\n",
    "2. Operator Penugasan\n",
    "digunakan untuk menetapkan nilai ke variabel.\n",
    "3. Operator Perbandingan\n",
    "Operator perbandingan digunakan untuk membandingkan dua nilai.\n",
    "4. Operator Logika\n",
    "adalah operator yang digunakan untuk operasi logika. Bentuk \n",
    "operator logika berupa kata hubung. Ada 3 kata hubung yang digunakan di \n",
    "operator logika yaitu and, or dan not.\n",
    "5. Operator Identitas\n",
    "digunakan untuk membandingkan objek, bukan jika mereka \n",
    "sama, tetapi jika mereka sebenarnya adalah objek yang sama, dengan lokasi \n",
    "memori yang sama.\n",
    "6. Operator Keanggotaan\n",
    "digunakan untuk menguji apakah urutan disajikan dalam \n",
    "suatu objek.\n",
    "7. Operator Bitwise\n",
    "adalah operator khusus untuk menangani operasi logika bilangan biner \n",
    "dalam bentuk bit. Bilangan biner sendiri merupakan jenis bilangan yang hanya\n",
    "terdiri dari 2 jenis angka, yakni 0 dan 1. Jika nilai asal yang dipakai bukan \n",
    "bilangan biner, akan dikonversi secara otomatis menjadi bilangan biner. Misalnya \n",
    "7 desimal = 0111 dalam bilangan biner. Pada penerapannya, operator bitwise \n",
    "tidak terlalu sering dipakai, kecuali anda sedang membuat program yang harus \n",
    "memproses bit-bit komputer. Selain itu operator ini cukup rumit dan harus \n",
    "memiliki pemahaman tentang sistem bilangan biner. Dalam bahasan kali ini saya \n",
    "menganggap anda sudah paham beda antara bilangan biner (basis 2) dan bilangan\n",
    "desimal (basis 10). Bahasa Python mendukung 6 jenis operator bitwise\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 41,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "6\n"
     ]
    }
   ],
   "source": [
    "#Contoh Operator Aritmatika \n",
    "a, b = 30, 5\n",
    "print(a // b)\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 43,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "25\n"
     ]
    }
   ],
   "source": [
    "#Contoh Operator Penugasan\n",
    "a, b = 20, 5\n",
    "a += b\n",
    "print(a)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 4,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "True\n"
     ]
    }
   ],
   "source": [
    "#Contoh Operator Perbandingan\n",
    "a, b = 20, 15\n",
    "print(a != b)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 47,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "nilai_1 and nilai_2= False\n",
      "nilai_1 and nilai_3= True\n"
     ]
    }
   ],
   "source": [
    "#Contoh Operator Logika \n",
    "#AND\n",
    "x < 10 and x < 25\n",
    "\n",
    "nilai_1 = True\n",
    "nilai_2 = False\n",
    "nilai_3 = True\n",
    "\n",
    "print(\"nilai_1 and nilai_2= \" + str(nilai_1 and \n",
    "nilai_2))\n",
    "print(\"nilai_1 and nilai_3= \" + str(nilai_1 and \n",
    "nilai_3))\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 44,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "False\n",
      "True\n"
     ]
    }
   ],
   "source": [
    "#Contoh Operator Identitas\n",
    "a, b = 20, 10\n",
    "print(a is b)\n",
    "print(a is not b)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 45,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "True\n",
      "False\n"
     ]
    }
   ],
   "source": [
    "#Contoh Operator Keanggotaan\n",
    "nama = \"faqih\"\n",
    "hoby = [\"bermain\", \"ngoding\", \"jalan-jalan\"]\n",
    "#cari huruf 'h' di variabel nama\n",
    "print('a' in nama)\n",
    "print('a' not in nama)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 46,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "x berisi angka 75 desimal atau 0b1001011 biner\n",
      "y berisi angka 50 desimal atau 0b110010 biner\n",
      "\n",
      "\n"
     ]
    },
    {
     "data": {
      "text/plain": [
       "'0b10'"
      ]
     },
     "execution_count": 46,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "#Contoh Operator Bitwise\n",
    "x = 75\n",
    "y = 50\n",
    "\n",
    "print('x berisi angka',x ,'desimal atau',bin(x),'biner')\n",
    "print('y berisi angka',y ,'desimal atau',bin(y),'biner')\n",
    "print('\\n')\n",
    "\n",
    "a = x & y\n",
    "bin(a)\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 1,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "460.1099999999999\n"
     ]
    },
    {
     "data": {
      "text/plain": [
       "float"
      ]
     },
     "execution_count": 1,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "#Soal No. 2\n",
    "X = (200 / 20 - 30) + (100*(21.9**2) / 100 + (10/20))\n",
    "\n",
    "print(X)\n",
    "\n",
    "type(X)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 16,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "0\n",
      "52\n",
      "-69\n",
      "x = 100 desimal dan 0b1100100 biner\n",
      "y = 10 desimal dan 0b1010 biner\n",
      "z = 68 desimal dan 0b1000100 biner\n"
     ]
    },
    {
     "data": {
      "text/plain": [
       "int"
      ]
     },
     "execution_count": 16,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "#SOAL No. 3 A, B, C\n",
    "x = 100\n",
    "y = 10\n",
    "z = 68\n",
    "print(x & y & z)\n",
    "print(x ^y << 5 >> 2)\n",
    "print(~x & ~y | ~z)\n",
    "\n",
    "print('x =', x ,'desimal dan', bin(x), 'biner')\n",
    "print('y =', y ,'desimal dan', bin(y), 'biner')\n",
    "print('z =', z ,'desimal dan', bin(z), 'biner')\n",
    "\n",
    "type(x)\n",
    "type(y)\n",
    "type(z)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 24,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "90.0\n",
      "545.5\n",
      "x = 100 desimal 0b1100100 biner\n",
      "y= 50 desimal 0b110010 biner\n",
      "z = 5 desimal 0b101 biner\n"
     ]
    },
    {
     "data": {
      "text/plain": [
       "int"
      ]
     },
     "execution_count": 24,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "#SOAL No. 4 A dan B\n",
    "x = 0b1100100\n",
    "y = 0b110010\n",
    "z = 0b101\n",
    "\n",
    "print(x - y / z)\n",
    "print(x*z +y / x-z +y)\n",
    "\n",
    "print('x =', x ,'desimal', bin(x), 'biner')\n",
    "print('y=', y ,'desimal', bin(y), 'biner')\n",
    "print('z =', z ,'desimal', bin(z), 'biner')\n",
    "\n",
    "type(x)\n",
    "type(y)\n",
    "type(z)"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3.10.7 64-bit",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.10.7"
  },
  "orig_nbformat": 4,
  "vscode": {
   "interpreter": {
    "hash": "96792473f43756a53da32662260be1b29f69eb983da56045868f1e3e212ccb09"
   }
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
