**NOTE**: for any "is_[...]" returns a boolean type variable
**NOTE**: for any "[...]_num" returns the value of f(x) given x
**NOTE**: for any "[...]_index" returns the value of x given f(x)

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

    int fibonacci_num(int num){
        int a = 0, b = 1, c = 0;
        
        for (int i=0; i<num; i++){
            a = b;
            b = c;
            c = a + b;
        }
        
        return c;
    }
}
