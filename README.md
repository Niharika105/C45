# C45
Structure with in structure 
#include<stdio.h>
struct data{
  int day,month,year;
  };
  struct student {
  char name[50];
  int rollno; 
  
  struct data dob;
};
int main(){
struct student s1={"Niharika",20,{7,10,2005}};
printf ("student name is %s\n",s1.name);
printf ("rollno:%d\n",s1.rollno);
printf("date of birth:%02d/%02d/%02d\n",s1.dob.day,s1.dob.month,s1.dob.year);
return 0;

}
