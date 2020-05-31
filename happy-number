class Solution {
public:
    bool isHappy(int n) {
        int res = 0;
        int temp = n,flag = 0;
        int arr[8] = {4,16,37,58,89,145,42,20}; 
        while(n != 0)
        {
            res += (n%10) * (n%10);
            
             n /= 10;  
        }   
        
        for(int i = 0; i < 8; i++)
            {
                if(res == arr[i]){
                    flag = 1;
                    break;
                }
            }
        if(flag == 1)
            return false;
        else{
            if(res == 1)
                return true;
            else
                return isHappy(res);
        }
    }
};
