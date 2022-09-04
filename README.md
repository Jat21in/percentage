# percentage
#include<stdio.h>
float percentage(float m1,float m2, float m3);
float total(float m1,float m2, float m3);
float main() {
   printf("****************** Welcome To Program To Display Student Grade *************************");
    printf("\n");
    char studentname[100] ;
    char studentclass[3];
    int rollno ;
    float m1;float m2; float m3;
    printf("Enter Student's Name :");
    fgets(studentname, 100 , stdin);

    printf("Enter Class :");
    fgets(studentclass , 3 ,stdin);
   
   printf("Enter Roll Number :");
   scanf("%d/n",& rollno);
    
    printf(" Enter Marks in 3 Subjects :\n");
    printf(" Marks in 1st Subjects :");
    scanf("%f/n",&m1);
    printf(" Marks in 2nd Subjects :");
     scanf("%f/n",&m2);
    printf(" Marks in 3rd Subjects :");
     scanf("%f/n",&m3);

   float t =total(m1,  m2,  m3);
   printf("Total Marks of Student is :%f\n",t);
   float p =percentage(m1,  m2,  m3);
   printf("Percentage of Student is :%f\n",p);

}
 float total(float m1, float m2, float m3) {
  return m1+m2+m3 ;

}

float percentage(float m1, float m2, float m3) {
  float p = ((m1+m2+m3)/3) ;
  return p;
}
