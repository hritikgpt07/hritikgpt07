- 👋 Hi, I’m @hritikgpt07
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
hritikgpt07/hritikgpt07 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
#include<process.h>
#include <stdio.h>
        void main(int argc,char *argv[])
 {

          FILE *fp1;
          int vowel=0,consonant=0;
          char ch;
          clrscr();
          if(argc!=2)
            {
                     printf("Insufficient Arguments");
                     exit(0);
            }
          fp1=fopen(argv[1],"r");
          if(fp1==NULL)
            {
                    printf("Source can't be opened");
                    exit(0);
            }
          ch=fgetc(fp1);
          while(ch!=EOF)
                {
                       if((ch=='a')||(ch=='A')||(ch=='e')||(ch=='E')||(ch=='i')||(ch=='I')||(ch=='o') ||(ch=='O')||(ch=='u')||(ch=='U'))
                         {
                               vowel++;
                          }
                      else
                         {
                             consonant++;
                         }
                             ch=fgetc(fp1);
                }
                             printf("\n Number of vowels are = %d",vowel);
                             getch();
}

