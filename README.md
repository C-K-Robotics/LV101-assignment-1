# LV101-assignment-1
In this assignment, you will write a LabVIEW program to calculate the price for a cake shop. You need to use your knowledge in variables, operators, and case structure to complish the assignment.
The files you need to modify are <code>cake_size.vi</code>, <code>discount.vi</code>, and <code>total.vi</code>. <br> After finishing these VIs, you can run the `main.vi` to testify your work. 

### <code>cake_size.vi</code>
This vi has five input variables: shape, r, a, b, and theta. The vi should calculate and output the size of the cake. 
- If the shape is "rectangle", the size would be $`a \times b`$.
- If the shape is "round", the size would be $`\pi r^{2}`$.
- If the shape is "triangle", calculates the size by the law of sines: $`\frac{1}{2} ab \sin{\theta}`$.
- If none of the cases above, outputs 0.

### <code>discount.vi</code></h3>
This vi has three input variables: size, flavor, and member. There are two kinds of discounts:
- The buyer is a member(member variable is true) and the cake is chocolate taste.
- The size is larger than 100 and the cake is not chocolate taste.
If either of the above cases is met, the vi should output 0.8 meaning a 20% discount. Otherwise, outputs 1 meaning the original price.

### <code>total.vi</code>
This vi has three input variables: size, discount, and count. The vi should output the total price which is the multiply of size, discount, and item count. However, the cake shop has a special "buy two get one free" discount. Thus, for every three cakes, the third cake would be free. So three cakes only charge the price of two, four cakes charge three, five cakes charge four, six cakes charge four, and so on. Round the price to nearest integer.
