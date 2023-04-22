# freq-coubt
First negative integer in every window of size “k”
![image](https://user-images.githubusercontent.com/98272915/233795160-7e32b7fd-61f2-4fc9-8669-83c30bb29e8f.png)
class Solution{
    public:
    //Function to count the frequency of all elements from 1 to N in the array.
    void frequencyCount(vector<int>& arr,int N, int P)
    { 
        unordered_map<int,int>mp;
        for(int i=0;i<N;i++){
            mp[arr[i]]++;
        }
        arr.clear();
        for(int i=1;i<=N;i++){
          arr.push_back(mp[i]);
        }
    }
};
