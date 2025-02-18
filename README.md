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
