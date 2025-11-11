# Cpplinear 
#include<iostream>
using namespace std;
int main()
{
	int n,i,rollno[10];
	cout<<"how many students attended the training program :";
	cin>>n;
	for( i=0;i<n;i++)
	{
		cout<<"enter roll no of student ";
		cin >> rollno[i];
	}
    cout<<"present roll no of students are:-";
    for( i=0;i<n;i++)
    {
    	cout<<rollno[i]<<" ";
	}
char b;
do
{
	int key;
	 cout << "\nEnter roll no of student to be checked: ";
     cin >> key;
     for (i = 0; i < n; i++)
     {
     	 if(rollno[i]==key)
         {
         	cout<<"the student is present";	
     	    break;
	     }
	 
	 if (rollno[i] != key)
	 {
	 	cout << "This student was absent" << endl;
	 	break;	
	 }
	
 
     
}
     cout<<"do you want to continue (y/n)";
     cin >> b;
	} while (b == 'y');
    
return 0;
}
