# substring
int main ()
{
  char string[50] ="my_name_is_edcast_future_skills";
  char substring[10][10];
  int i,j=0,cnt=0;
  int p=strlen(string);
  printf ("String  \"%s\" is split into substrings:\n",string);
  for(i=0;i<=p;i++)
  {
  	if(string[i]=='_'||string[i]=='\0')
  {
  	  substring[cnt][j]='\0';
	  cnt++;
  	  j=0;
  }
  	else
  {
	
	  substring[cnt][j]=string[i];
	  j++;
  }
 } 
 for(i=0;i<cnt;i++)
 {
 printf("%s\n",substring[i]);
 }
 return 0;
}
