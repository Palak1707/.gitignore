# .gitignore
TestVagrant Coding Assesment 

Java Code : 

#include <iostream>
using namespace std;
int main()
{
    float toi, hindu, et, bm, ht;
    toi = 27;
    hindu = 18;
    et = 34;
    bm = 10.5;
    ht = 18;
    float arr[5] = {toi, hindu, et, bm, ht};
    int input;
    cin >> input;
    for (int i = 0; i < 5; i++)
    {
        for (int j = i + 1; j < 5; j++)
        {
            if (arr[i] + arr[j] <= input)
            {
                switch (i)
                {
                case 0:
                    cout << "{\"TOI\", ";
                    break;

                case 1:
                    cout << "{\"Hindu\", ";
                    break;

                case 2:
                    cout << "{\"ET\", ";
                    break;

                case 3:
                    cout << "{\"BM\", ";
                    break;

                case 4:
                    cout << "{\"HT\", ";
                    break;
                }
                switch (j)
                {
                case 0:
                    cout << "\"TOI\"}, ";
                    break;

                case 1:
                    cout << "\"Hindu\"}, ";
                    break;

                case 2:
                    cout << "\"ET\"}, ";
                    break;

                case 3:
                    cout << "\"BM\"}, ";
                    break;

                case 4:
                    cout << "\"HT\"}, ";
                    break;
                }
            }
        }
    }
    return 0;
}
                              
------------------------------------------------------------------------------------------------------------------------------------------------------------------                              
C++ Code : 
                              
class Solution 
{
  public:
     vector <string> letterCombinations (String digits)
     {
        if (!digits.size())
         {
           return();
         }
        vector <string> combs;
        const vector <string> TOI = {"3","3","3","3","3","5","6"};
        const vector <string> Hindu = {"2.5","2.5","2.5","2.5","2.5","4","4"};
        const vector <string> ET = {"4","4","4","4","4","4","10"};
        const vector <string> BM = {"1.5","1.5","1.5","1.5","1.5","1.5","1.5"};
        const vector <string> HT = {"2","2","2","2","2","4","4"};
     };
   string builder;
   build (builder, 0, digit, TOI, Hindu, ET, BM, HT, combs);
   return combs;
  }
  void build(string builder, int i,conts string & digit, const vector <string> & TOI,const vector <string> & Hindu, const vector <string> & ET, const vector <string> &  BM, const vector <string> & HT, vector <string> & combs)
  {
    if (i==digits.size)
    {
      combs.push_back(builder);
      return;
    }
    int d = digits[i]-'0';
    for (char ch:TOI[d])
    {
      build(builder+ch, i+1, digits, TOI, combs);
    }
    for (char ch:Hindu[d])
    {
      build(builder+ch, i+1, digits, Hindu, combs);
    }
    for (char ch:ET[d])
    {
      build(builder+ch, i+1, digits, ET, combs);
    }
    for (char ch:BM[d])
    {
      build(builder+ch, i+1, digits, BM, combs);
    }
    for (char ch:HT[d])
    {
      build(builder+ch, i+1, digits, HT, combs);
    }
  }
 };
  
  
  Word FIle folder : 
  
[Palak Shrivastava.docx](https://github.com/Palak1707/.gitignore/files/10306362/Palak.Shrivastava.docx)

