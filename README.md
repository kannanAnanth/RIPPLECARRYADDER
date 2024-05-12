# RIPPLECARRYADDER
![image](https://github.com/RESMIRNAIR/RIPPLECARRYADDER/assets/154305926/62459000-90cb-4c43-a221-7b8cf1d419b0)
![image](https://github.com/RESMIRNAIR/RIPPLECARRYADDER/assets/154305926/24ea1940-0b55-4f8a-be6a-a7ac5daf2919)
# Full Adder
![image](https://github.com/RESMIRNAIR/RIPPLECARRYADDER/assets/154305926/3208d46f-2fd4-4d6a-987f-63102c173ca0)

# Program
```
module fa(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = a^b^c;
assign carry=(a&b)|(b&c)|(c&a);
endmodule
module rca(a,b,cin,sum,cout);
input [3:0]a,b;
input cin;
output [3:0]sum;
output cout;
wire c1,c2,c3;
fa fa1(a[0],b[0],cin,sum[0],c1);
fa fa2(a[1],b[1],c1,sum[1],c2);
fa fa3(a[2],b[2],c2,sum[2],c3);
fa fa4(a[3],b[3],c3,sum[3],cout);
endmodule

```
# Output
![WhatsApp Image 2024-05-12 at 18 03 29_c0d15eda](https://github.com/kannanAnanth/RIPPLECARRYADDER/assets/160721190/172e1bf3-9cd8-418b-a31c-b04b40845286)

# Result
 Ripplecarryadder output has verified

