# OOP_Report_0411

#include <stdio.h>
#define arrSize 16
int main() {
int hex;
printf("16진수로 입력받을 수를 입력하세요: ");
scanf("%x", &hex);
int bit[arrSize] = {0};
int i = 0;
while (hex > 0) {
bit[i] = hex % 2;
hex /= 2;		
i++;
}
for (i = 15; i>11; i--){
printf("%d",bit[i]);
}
printf(" : ");
for(i = 11; i>8; i--){
printf("%d",bit[i]);
}
printf(" : ");
for(i = 8; i>=0; i--){
printf("%d",bit[i]);
}    
return 0;
}
