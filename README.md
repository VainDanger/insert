#include<iostream>

void insert_sorting(int nu[])
{
  for(int i=1; i<4; i++)
    {
      for(int j=i; nu[j]<nu[j-1] and j>0; j--)  std::swap(nu[j],nu[j-1]);
    }
  for(int i=0; i<4; i++)  std::cout<<nu[i]<<' ';
}

int main(void)
{ 
  int nu[4]{1,2,4,3};
  insert_sorting(nu);
}
