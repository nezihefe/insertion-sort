#include<stdio.h>
#include <time.h>
int main(){
  int karsilastirma=0,yerdegistirme=0;
  int i,j,s,temp,a[20];

  printf("Enter total elements: ");
  scanf("%d",&s);

  printf("Enter %d elements: ",s);
  for(i=0;i<s;i++)
      scanf("%d",&a[i]);
clock_t start = clock();
  for(i=1;i<s;i++){
      temp=a[i];
      j=i-1;
      karsilastirma+=1;
      while((temp<a[j])&&(j>=0)){
      yerdegistirme+=1;
      a[j+1]=a[j];
          j=j-1;
      }
      a[j+1]=temp;
  }
clock_t stop = clock();
    double elapsed = (double)(stop - start) * 1000.0 / CLOCKS_PER_SEC;
  printf("After sorting: ");
  for(i=0;i<s;i++)
      printf(" %d",a[i]);
printf("Gecen sure: %f\n", elapsed);
printf("karsilastirma= %d\n",karsilastirma);
printf("yerdegistirme= %d\n",yerdegistirme);
  return 0;
}
