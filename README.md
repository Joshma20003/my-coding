# my-coding
//program to find average thurst of rocket





#include <stdio.h>
//force=weight*velocity/gravity*time
//thrust=weight+force
void force(float*,float*,float*);
void thrust(float*,float*);
float f,th;
int main()
{
	float weight,velocity,time;
	printf("enter the values of weight,velocity,time\n");
	scanf("%f %f %f",&weight,&velocity,&time);
	force(&weight,&velocity,&time);
	thrust(&weight,&f);
	printf("force=%f\nthrust=%f\n",f,th);
	return 0;
}
void force(float *w,float *v,float *t)
{
	float g= 32.2;
	f=((*w)*(*v))/((g)*(*t));
}
void thrust(float *w,float*f)
{
	th=*w+(*f);
}
