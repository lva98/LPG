#include <iostream>
#include <string>
using namespace std;
int main(){
    string word1, word2;
    int a, cont=0;
    cin >> a;
    while(a--){
        cin >> word1 >> word2;
        if(word1.size() >= word2.size()){
            for(int i=0; i<word2.size(); i++){
                cout << word1[i];
                cout << word2[i];
                cont++;
            }
            if(cont < word1.size()-1){
                for(int i=cont+1; i<word1.size()-1; i++){
                    cout << word1[i];
                }
            }
        cout << endl;
        cont = 0;
        }
        else{
            for(int i=0; i<word1.size(); i++){
                cout << word1[i];
                cout << word2[i];
                cont++;
            }
            for(int i=cont+1; i<word2.size()-1; i++){
                cout << word2[i];
            }
        cout << endl;
        cont = 0;
        }
    }
}
