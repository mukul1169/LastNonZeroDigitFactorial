
static int lastNonZeroDigit(int n) {
       // Write your code here
       int f=1;
       for(int i=1;i<=n;i++)
           f=f*i;
       int ans=0;
       while(f>0)
       {
           ans=f%10;   
           if(ans!=0)
              return ans;
           else
             f=f/10;
       }
       return ans;
   }
