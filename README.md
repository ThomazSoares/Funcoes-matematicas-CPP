**NOTE**: for any "is_[...]" returns a boolean type variable

{

    int is_prime(int num){
        int cond = 1;
        
        if ((num == 1 || num == 0 || num % 2 == 0) && num != 2){
            cond = 0;
        } else{
            for (int i=3; i<num; i+=2){
                if (num % i == 0){
                    cond = 0;
                    break;
                }
            }
        }
        
        return cond;
    }
}
