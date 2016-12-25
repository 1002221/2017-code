# 2017-code


#include <stdio.h>

int plus(int a, int b);
int minus(int a, int b);
int times2(int a, int b);
int divby(int a, int b);

typedef int (*p_fun)(int a, int b);

int main()
{
    int a = 1, b = 2, c=3, d=4, e=5, f=6, g=7, h=8, h1=9, h2=10;
    p_fun pa[] = {plus, minus, times2, divby};
    
        for( int q = 0; q < sizeof(pa)/sizeof(p_fun); q++ ){
            for( int p = 0; p < sizeof(pa)/sizeof(p_fun); p++ ){
                for( int o = 0; o < sizeof(pa)/sizeof(p_fun); o++ ){
                    for( int n = 0; n < sizeof(pa)/sizeof(p_fun); n++ ){
                        for( int m = 0; m < sizeof(pa)/sizeof(p_fun); m++ ){
                            for( int l = 0; l < sizeof(pa)/sizeof(p_fun); l++ ){
                                for( int k = 0; k < sizeof(pa)/sizeof(p_fun); k++ ){
                                    for( int j = 0; j < sizeof(pa)/sizeof(p_fun); j++ ){
                                        for( int i = 0; i < sizeof(pa)/sizeof(p_fun); i++ ){
                                            if(pa[q](pa[p](pa[o](pa[n](pa[m](pa[l](pa[k](pa[j](pa[i](a,b),c),d),e),f),g),h),h1),h2)==2017){
                                                printf("%d,%d,%d,%d,%d,%d,%d,%d,%d,%d,%d,%d,%d,%d,%d,%d,%d,%d,%d\n",a,i,b,j,c,k,d,l,e,m,f,n,g,o,h,p,h1,q,h2);
                                            }
                                        }}}}}}}}}
    return 0;
}

int plus(int a, int b){
    return a+b;
}

int minus(int a, int b){
    return a-b;
}

int times2(int a, int b){
    return a*b;
}

int divby(int a, int b){
    return a/b;
}
