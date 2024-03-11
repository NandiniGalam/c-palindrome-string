# c-palindrome-string
include <stdio.h>
#define MAX_SIZE 100
int main() 
{
  char str[MAX_SIZE];
  int len, startindex, endindex;
  printf("enter any string: ");
  scanf("%s",str);
  len = 0;
  while(str[len]!='\0') len ++;
  startindex = 0;
  endindex = len-1;
  while(startindex <= endindex)
  {
    if(str[startindex] != str[endindex])
    break;
    startindex++;
    endindex--;
  }
  if(startindex >=endindex)
  {
    printf("STRING IS PALINDROME. ");
  }
  else
  {
  printf("string is not a palindrome.");
  return 0;
  }
}
    
  
  
