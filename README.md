## โจทย์
เขียนคำสั่งในการสร้างและเรียกใช้ฟังก์ชัน GetMatrix() เพื่อรับจำนวนแถว คอลัมน์ และค่าของแต่ละสมาชิกในเมทริกซ์จากคีย์บอร์ดตามโปรโตไทป์ต่อไปนี้

## ข้อบังคับ
1. ต้องกรอกรายละเอียดของตนเองในไฟล์ `student_info.txt` โดยมีข้อมูลสำคัญที่ต้องกรอกคือ
   - รหัสนักศึกษา เช่น 678888888-8
   - รหัสวิชา เช่น ENGCE117
   - เทอมที่เรียน เช่น 2/2567
2. ต้องสร้างไฟล์ชื่อ `student_program.c` และทำการเขียนโค้ดโปรแกรมของนักศึกษาลงไปในไฟล์นี้

## FIX CODE
```c++
#include <stdio.h>

void GetMatrix( int value[], int *row, int *col ) ;

int main() {
    int *data, m, n ;
    GetMatrix( &data, &m, &n ) ;
    for( int i = 0 ; i < m ; i++ ) {
      for( int j = 0 ; j < n ; j++ ) {
          printf( "%d ", data[i][j] ) ;
      }
      printf( "\n" ) ;
    }
    return 0 ;
}//end function
```

## TEST CASE 1
### Input
```bash
Enter the number of rows: 2
Enter the number of columns: 3
Enter the matrix elements: 1 2 3 4 5 6
```
### Output
```bash
Matrix (2x3):
1 2 3
4 5 6
```

## TEST CASE 2
### Input
```bash
Enter the number of rows: 3
Enter the number of columns: 2
Enter the matrix elements: 7 8 9 10 11 12
```
### Output
```bash
Matrix (3x2):
7 8
9 10
11 12
```
