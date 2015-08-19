#include<stdio.h>
int main()
	{
		float n,x[10]={0,0,0,0,0,0,0,0,0,0},y[10],A[10]={0,0,0,0,0,0,0,0,0,0},mul=1,q[10]={0,0,0,0,0,0,0,0,0,0};
		int i,j,k=0,p=0,m=0,sum=0,s;
		printf("\n enter the number of entries(maximum 5)\n");
		scanf("%f",&n);
		if(n<=5)
		{
		printf("\n enter the values of x\n");
		for(i=0;i<n;i++)
		{
			scanf("%f",&x[i]);
		}
		printf("\n enter the corresponding values of y\n");
		for(i=0;i<n;i++)
		{
			scanf("%f",&y[i]);
		}
		
		
		for(j=0;j<n;j++)
		{mul=1;
		for(i=0;i<n;i++)
		{
			if(i!=j)
			mul=mul*(x[j]-x[i]);
		}
		q[j]=y[j]/mul;
		}
		for(i=0;i<n;i++)
		{
			A[0]=A[0]+q[i];
		}
			
		for(j=0;j<n;j++)
		{
		A[1]=A[1]+(q[j]*(x[0]+x[1]+x[2]+x[3]+x[4]+x[5]-x[p]));
		p++;		
		}B:
		sum=0;
		for(i=0;i<n;i++)
		{
		for(j=i;j<n;j++)
		{
			if(i!=j&&(j!=m&&i!=m))
			{
				sum=sum+(x[i]*x[j]);
			}
		}
		
		}
		A[2]=A[2]+(q[m]*sum);
		m++;
		if(m!=n)
		goto B;
		m=0;
		G:
		sum=0;
		for(i=0;i<n;i++)
		{
		for(j=i;j<n;j++)
		{
		for(k=j;k<n;k++)
			{
				if(i!=j&&i!=k&&j!=k&&j!=m&&i!=m&&k!=m)
			{
				sum=sum+(x[i]*x[j]*x[k]);
			}
		}
		
		
		}}
		A[3]=A[3]+(q[m]*sum);
		m++;
		if(m!=n)
		goto G;
		m=0;
		T:
		for(i=0;i<n;i++)
		{
			for(j=i;j<n;j++)
			{
				for(k=j;k<n;k++)
				{
				for(p=k;p<n;p++)
				{
				if(i!=m&&j!=m&&i!=j&&k!=m&&i!=k&&j!=k&&p!=i&&p!=j&&p!=k&&p!=m)
				{
					A[4]=A[4]+(q[m]*x[j]*x[i]*x[k]*x[p]);


				}
				}
			}
		}}
		m++;
		if(m!=n)
		goto T;


		printf("\n the function is\ny=");
		


		p=n-1;
		s=2;
		for(i=0;i<n;i++)
		{	
			
			if(A[i]!=0)
			{
			if(s%2==0)
			printf("+ %.2fx^%d ",A[i],p);
			
			else
			{
			A[i]=A[i]*-1;
			if(A[i]>=0)
			printf("+ %.2fx^%d ",A[i],p);
			else
			printf(" %.2fx^%d ",A[i],p);
			}
			
			}
			
			p--;
			s++;
			
		
		}
			printf("\n");
			}
		else 
		{
			printf("\nsorry the program works for a maximum of 5 entries\n");
		}
	return 0;
}
