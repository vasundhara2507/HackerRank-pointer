#include <stdio.h>

void update(int *a,int *b) {
    // Complete this function 
int sum=*a+*b;
int dif;
if(*a>*b){
    dif=*a-*b;
}
else if(*b>*a){
    dif=*b-*a;
}
*a=sum;
*b=dif;
}

int main() {
    int a, b;
    int *pa = &a, *pb = &b;
    
    scanf("%d %d", &a, &b);
    update(pa, pb);
    printf("%d\n%d", a, b);

    return 0;
}
