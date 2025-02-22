Stting Concepts:

#include <iostream>
#include <vector>
#include <algorithm>
#include <string>
using namespace std;
/*
void Reversechar(vector<char>&s){
    int n=s.size();
    int st=0;
    int end=n-1;
while(st<end){
    swap(s[st],s[end]);
    st++;
    end--;
}
}

//int main(){
//     char str[100];
//     cout<<"entr the string array :";
//     cin.getline(str,100,'$')>>str;

//     cout<<"output :"<<str<<endl;
// vector<char>s={'n','i','k'};

// Reversechar(s);
// for(char sti:s){
// cout<<sti<<"  ";
// }
// cout<<endl;

 //}
 bool isAlphaNum(char ch){
if((ch>='0' && ch<='9') || (tolower(ch)>='a' && (tolower(ch)<='z'))){
    return true;
}
return false;
 }
bool isPalindrome(string s){
    int st=0;
    int end=s.length()-1;
    while(st<end){
        if(!isAlphaNum(s[st])){
            st++;
            continue;
        }
        if(!isAlphaNum(s[end])){
            end++;
            continue;
        }
        if(tolower(s[st])!=tolower(s[end])){
            return false;
        }
        st++;
        end--;
    }
    return -1;
}
 int main(){
    string s="Nikhl";
   cout<< isPalindrome( s);

 }
   */
//   void occurance(string s,string sub){
  
    
//     if(s.find(sub)<s.length()){
       
//         s.erase(s.find(sub),s.length());
//     }
//     return -1;
//   }
//   int main(){
//     string s="daabcaabcbc";
//     string sub="abc";
//     cout<<occurance(s,sub);
//   }

/*
bool  isFreqsame(int freq1[],int freq2[]){
    for(int i=0;i<26;i++){
        if(freq1[i]!=freq2[i]){
            return false;
        }
    }
    return true;
}
checkinclusion(string s1,string s2){
    int freq[26]={0};
    for(int i=0;i<s1.length();i++){
        freq[s1[i]-'a']++;
    }
    int windsize=s1.length();
    for(int i=0;i<s2.length();i++){
        int windIdx=0;
        int idx=i;
        int windfreq[26]={0};

        while(windIdx<windsize && idx <s2.length()){
            windfreq[s2[idx]-'a']++;
            windIdx++;idx++;
        }
        if(isFreqsame(freq,windfreq)){
            return true;
        }
        return false;
    }
}

int main(){

 string s1="ab";
   string s2="yetabygds";
   checkinclusion(s1,s2);

   
}
 

  string reversestring(string s){
    int n=s.length();
    string ans="";//The pen
    reverse(s.begin(),s.end());
    //nep ehT
    for(int i=0;i<n;i++){
        string word="";
        while(i<n && s[i]!=' '){
            word+=s[i];//valid char
            i++;
        }//remove the spaces
        reverse(word.begin(),word.end());
  
        if(word.length()>0){
            ans+=" "+word;
        }
        
    }
    return ans.substr(1);
   }
int main(){
    string s="Nikhil Ahire";
    reversestring(s);
    string reversed = reversestring(s);
    cout << reversed << endl;
    return 0;
}

     void strcount(char arr){
        int n=arr.size();
        int count=0;
        int idx=i;
        for(int i=0;i<n;i++){
           
            char curr_char=0;
        while(n>i && arr[i]!=n+1){
            curr_char==arr[i];
            count++;
            idx++;
        }

        }
     }
int main(){
    char arr[]='a','a','b','b','c','c','c';
    strcount(arr);
}

  char   tolowerCase(char ch){
    if(ch>='a' && ch<='z'){
        return ch;
    }
    else{
        char temp=ch-'A'+'a';
        return temp;
    }
  }
int main(){
    char c='C';
cout<<tolowerCase(c);
}
   
    


   bool valid(char ch){
    if ((ch >= 'a' && ch <= 'z') || (ch >= 'A' && ch <= 'Z') || (ch >= '0' && ch <= '9')) {

            return 1;
        }
        else{
            return 0;
        }

      }
      char tolowerCase(char ch){
        if((ch>='a' && ch<='z') || (ch >= '0' && ch <= '9')){
            return ch;
        }
        else{
            char temp=ch-'A'+'a';
            return temp;
        }
      }
      bool checkpal(string s){
        int st=0;
        int end=s.length()-1;
        while(st<=end){
            if(s[st]!=s[end]){
                return false;
            }
            else{
                st++;
                end--;
            }
        }return true;
      }
     string removefaltuchar(string s){
        int i=0;
        string result="";
        for(int j=0;j<s.length();j++){
           if (valid(s[j])){
           result.push_back(s[j]);
           }
            
        }
        for(int j=0;j<result.length();j++){

            result[j]=tolowerCase(result[j]);
        }
        return checkpal(result) ? `"true"`: "false"; 
      }
      int main(){
        string s="ab@cdcba";
        cout<<removefaltuchar(s);
      }
       
bool  isFreqsame(int freq1[],int freq2[]){
    for(int i=0;i<26;i++){
        if(freq1[i]!=freq2[i]){
            return false;
        }
    }
    return true;
}
checkinclusion(string s1,string s2){
    int freq[26]={0};
    for(int i=0;i<s1.length();i++){
        freq[s1[i]-'a']++;
    }
    int windsize=s1.length();
    for(int i=0;i<s2.length();i++){
        int windIdx=0;
        int idx=i;
        int windfreq[26]={0};

        while(windIdx<windsize && idx <s2.length()){
            windfreq[s2[idx]-'a']++;
            windIdx++;idx++;
        }
        if(isFreqsame(freq,windfreq)){
            return true;
        }
        return false;
    }
}

int main(){

 string s1="ab";
   string s2="yetabygds";
   checkinclusion(s1,s2);

   
}
 


   char strcomp(char ch){
    char n=ch.size();
    int index=0;
    int i=0;
    while(i<n){
        char curr_char=ch[i];
        count=0;
        while(i<n && ch[i]==curr_char){
           count++;
           i++;

        }
        ch[index]=curr_char;//No do the assign work
        index++;
        if(count>1){
            string count_str=to_string(count);
            for(char &ch1:count_str){
                ch[index]=ch1;
                index++;
            }
        }
    }
    return i;

   }
  int main(){
    char ch={'a','a','b','b','c'};

    strcomp(ch);
  }

      
     
  char maxoccChar(string s,int n){
      int arr[26]={0};

      //create an array of count of characters
        for(int i=0;i<n;i++){
           char ch=s[i];
             int num=0;
             if(ch >='a' && ch<='z'){
                num=ch-'a';
             }
             else{
                num=ch-'A';
             }
            
                
                arr[num]++;
            
           
           
        }
       // find max occ charcter
        int max=-1;int ans=0;
        for(int i=0;i<26;i++){
            if(max<arr[i]){
                ans=i;
               max=arr[i];

            }
        }
        char res='a'+ans;
        return res ;
     }
     int main()
     {
        string s="nikhil";
        int n=s.length();
        cout<<maxoccChar(s,n);
     }
        

      string adspcialchar(string ch){
        string result="";
        for(int i=0;i<ch.length();i++){
           
            if(ch[i]==' '){
               result.push_back('@') ;
               result.push_back('#') ;
            }
            else{
                result.push_back(ch[i]);
            }
        }
        return result;
      }
    int main(){
        string ch="nikhil ahire";
        cout<<adspcialchar(ch);
    }
        */

//panagram sentence english char apears at only onece
#include <iostream>
#include <string>
using namespace std;

bool isPangram(string ch) {
    int arr[26] = {0};
int count=0;
    for (char s : ch) {
        if (s >= 'a' && s <= 'z') {
            int num = s - 'a';
            arr[num]++;
            count++;
        }
    }

    // for (int i = 0; i < 26; i++) {
    //     if (arr[i] == 0) {
    //         return false;
    //     }
    // }
    if(count==26){
        return true;
    }
    return false;
}

int main() {
    string ch = "thequickbrownfo";
    if (isPangram(ch)) {
        cout << "The string is a pangram." << endl;
    } else {
        cout << "The string is not a pangram." << endl;
    }
    return 0;
}


remaining part of strings -->
   bool valid(char ch){
    if ((ch >= 'a' && ch <= 'z') || (ch >= 'A' && ch <= 'Z') || (ch >= '0' && ch <= '9')) {

            return 1;
        }
        else{
            return 0;
        }

      }
      char tolowerCase(char ch){
        if((ch>='a' && ch<='z') || (ch >= '0' && ch <= '9')){
            return ch;
        }
        else{
            char temp=ch-'A'+'a';
            return temp;
        }
      }
      bool checkpal(string s){
        int st=0;
        int end=s.length()-1;
        while(st<=end){
            if(s[st]!=s[end]){
                return false;
            }
            else{
                st++;
                end--;
            }
        }return true;
      }
     string removefaltuchar(string s){
        int i=0;
        string result="";
        for(int j=0;j<s.length();j++){
           if (valid(s[j])){
           result.push_back(s[j]);
           }
            
        }
        for(int j=0;j<result.length();j++){

            result[j]=tolowerCase(result[j]);
        }
        return checkpal(result) ? `"true"`: "false"; 
      }
      int main(){
        string s="ab@cdcba";
        cout<<removefaltuchar(s);
      }
       
bool  isFreqsame(int freq1[],int freq2[]){
    for(int i=0;i<26;i++){
        if(freq1[i]!=freq2[i]){
            return false;
        }
    }
    return true;
}
checkinclusion(string s1,string s2){
    int freq[26]={0};
    for(int i=0;i<s1.length();i++){
        freq[s1[i]-'a']++;
    }
    int windsize=s1.length();
    for(int i=0;i<s2.length();i++){
        int windIdx=0;
        int idx=i;
        int windfreq[26]={0};

        while(windIdx<windsize && idx <s2.length()){
            windfreq[s2[idx]-'a']++;
            windIdx++;idx++;
        }
        if(isFreqsame(freq,windfreq)){
            return true;
        }
        return false;
    }
}

int main(){

 string s1="ab";
   string s2="yetabygds";
   checkinclusion(s1,s2);

   
}
 


   char strcomp(char ch){
    char n=ch.size();
    int index=0;
    int i=0;
    while(i<n){
        char curr_char=ch[i];
        count=0;
        while(i<n && ch[i]==curr_char){
           count++;
           i++;

        }
        ch[index]=curr_char;//No do the assign work
        index++;
        if(count>1){
            string count_str=to_string(count);
            for(char &ch1:count_str){
                ch[index]=ch1;
                index++;
            }
        }
    }
    return i;

   }
  int main(){
    char ch={'a','a','b','b','c'};

    strcomp(ch);
  }

      
     
  char maxoccChar(string s,int n){
      int arr[26]={0};

      //create an array of count of characters
        for(int i=0;i<n;i++){
           char ch=s[i];
             int num=0;
             if(ch >='a' && ch<='z'){
                num=ch-'a';
             }
             else{
                num=ch-'A';
             }
            
                
                arr[num]++;
            
           
           
        }
       // find max occ charcter
        int max=-1;int ans=0;
        for(int i=0;i<26;i++){
            if(max<arr[i]){
                ans=i;
               max=arr[i];

            }
        }
        char res='a'+ans;
        return res ;
     }
     int main()
     {
        string s="nikhil";
        int n=s.length();
        cout<<maxoccChar(s,n);
     }
        

      string adspcialchar(string ch){
        string result="";
        for(int i=0;i<ch.length();i++){
           
            if(ch[i]==' '){
               result.push_back('@') ;
               result.push_back('#') ;
            }
            else{
                result.push_back(ch[i]);
            }
        }
        return result;
      }
    int main(){
        string ch="nikhil ahire";
        cout<<adspcialchar(ch);
    }
      
//panagram sentence english char apears at only onece
#include <iostream>
#include <string>
using namespace std;

bool isPangram(string ch) {
    int arr[26] = {0};
int count=0;
    for (char s : ch) {
        if (s >= 'a' && s <= 'z') {
            int num = s - 'a';
            arr[num]++;
            count++;
        }
    }

    // for (int i = 0; i < 26; i++) {
    //     if (arr[i] == 0) {
    //         return false;
    //     }
    // }
    if(count==26){
        return true;
    }
    return false;
}

int main() {
    string ch = "thequickbrownfo";
    if (isPangram(ch)) {
        cout << "The string is a pangram." << endl;
    } else {
        cout << "The string is not a pangram." << endl;
    }
    return 0;
}
     

      int main(){
        int n=3;
        for(int i=2;i*i<=n;i++){
            if(n%i==0){
                cout<<"non prime";
            }
            
        }
        cout<<"prime";
      }
        
       string countandSay(int n){

        if(n==1){
            return "1";
        }
        string say= countandSay(n-1);
        string result="";
       for(int i=0;i<say.length();i++){
       int count=1;
      char ch=say[i];
       //process
       while(i<say.size()-1 && say[i]==say[i+1]){
        count++;
        i++;
       }
       result+=to_string(count)+ string(1,ch);
       }
       return result;

        }
         int main(){ 
            int n=4;
            cout<<countandSay(n);
         }
// for n = 4:
// n = 4, so countandSay(4) is called.

// countandSay(4) calls countandSay(3), which calls countandSay(2), which calls countandSay(1).

// countandSay(1) returns "1".

// Now, countandSay(2) processes "1":

// Result becomes "11" (one "1").

// Then, countandSay(3) processes "11":

// Result becomes "21" (two "1"s).

// Finally, countandSay(4) processes "21":

// Result becomes "1211" (one "2", one "1").

int countPrime(int n){
    vector <bool>isPime(n+1,true);
        int count=0;
        for(int i=2;i<n;i++){
            if(isPime[i]){
                count++;
                for(int j=i*2;j<n;j+i){
                    isPime[j]=false;
                
            }
        }
       
    }
    return count;
}
int main(){
    int n=50;
    cout<<countPrime(n);
   
}
 
   string intToroman(vector<int> &val,vector<string>&sym,int num){
    string result="";
    for(int i=0;i<13;i++){
              while(val[i]<=num ){
                if(num==0){
                    break;
                }
                int times=num/val[i];
                while(times--){
                    result+=sym[i];
                }
                num=num%val[i];
              }
              
        }
        return result;
       
    };
    int main(){
        static vector<int>val={1000,900,500,400,100,90,50,40,10,9,5,4,1};
       static vector<string>sym={"M","CM","D","CD","C","XC","L","XL","X","IX","V","IV","I"};
       
        int num=1994;
        cout<<intToroman(val,sym,num);
    }

           bool Eqstring(vector<string>&w1,vector<string>&w2){
            string store1="";
            string store2="";
            for(int i=0;i<w1.size() && i<w2.size();i++){
               
           
            if(w1.size()>0){
                store1+=w1[i];
            }
            if(w2.size()>0){
                store2+=w2[i];
            }
           
            return store1==store2;
        }
           }
int main(){
   vector<string>w1={"ab","c"};
   vector<string>w2={"a","bc"};
   cout << (Eqstring(w1, w2) ? "true" : "false");
}
  
  Eqstring(vector<string>&w1,vector<string>&w2){
   int m= w1.size();
   int n=w2.size();
    int w1i=0;
    int i=0;
    int w2i=0;
    int j=0;
    while(w1i<m && w2i<n){
        if(w1[w1i][i] !=w2[w2i][w2]){
            return false;
        }
        i++;
        J++;
        if(i==w1[w1i].length()){
            i=0;
            w1i++;

        }
        if(j==w2[w2i].length()){
            j=0;
            w2i++;

        }
    }
    if(w1i==w1.size() && w2i==w2size() ){
        return true;

    }
    return false;
    
  }
  int main(){
    vector<string>w1={"ab","c"};
    vector<string>w2={"a","bc"};
    cout << Eqstring(w1, w2) ;
  }
