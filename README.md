# -c++-
//2015年解决的OJ问题
//A除以B的问题
#include"iostream"
#include "string"
using namespace std;
int main()
{
	string A,Q;
	int B,R,j,i,s;
	i=0;
	do 
	{
		cin>>A[i];
		i++;
	} while (A[i-1]=='0');
	
	j=A.size();
	
	cin>>B;
	if ((A[0]-'0')>=B)
	{
		 s=j;
		 for (i=0;i<s;i++)
		 {
			
			 R=(A[i]-'0')%B;
			 A[i+1]=R*10+A[i+1];
			 Q[i]=(A[i]-'0')/B+'0';
		 }

	}
	else 
	{
		 s=j-1;
		 for (i=0;i<s;i++)
		 {
			 R=(A[i]-'0')%B;
			 A[i+1]=R*10+A[i+1];
			 Q[i]=(A[i+1]-'0')/B+'0';
		 }
	}
	for (i=0;i<s;i++)
	{
		cout<<Q[i];
	}
	cout<<R;
	system("pause");
	return 0;
}
