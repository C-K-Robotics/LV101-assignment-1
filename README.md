<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=">
    <title>LV101-assignment-1</title>
</head>

<body>
    <h1>LV101-assignment-1</h1>
    <div>
        <h2>Exercise #1</h2>
        <p>In this exercise, you will write a LabVIEW program to calculate the price for a cake shop. You need to use your knowledge in variables, operators, and case structure to complish the assignment.</p>
        <p>The files you need to modify are cake_size.vi, discount.vi, and total.vi <br> After finishing these vi, you can run the main.vi to testify your work. main.vi cannot be modified.</p>
        <div>
            <h3>cake_size.vi</h3>
            <p>This vi has five input variables: shape, r, a, b, and theta. The vi should calculate and output the size of the cake. If the shape is "rectangle", the size would be <math display="inline"><mi>a</mi><mo>*</mo><mi>b</mi></math>. If the shape is "round", the size would be <math display="inline"><mfrac><mn>1</mn><mn>2</mn></mfrac><mi>π</mi><msup><mi>r</mi><mn>2</mn></msup></math>. If the shape is "triangle", calculates the size by the law of sines: <math display="inline"><mfrac><mn>1</mn><mn>2</mn></mfrac><mi>a</mi><mi>b</mi><mi>sin θ</mi></math>. If none of the cases above, outputs 0.</p>
        </div>
        <div>
            <h3>discount.vi</h3>
            <p>This vi has three input variables: size, flavor, and member. There are two kinds of discounts:
            <ol>
                <li> The buyer is a member(member variable is true) and the cake is chocolate taste.</li>
                <li>The size is larger than 100 and the cake is not chocolate taste.</li>
            </ol>
            If either of the above cases is met, the vi should output 0.8 meaning a 20% discount. Otherwise, outputs 1 meaning the original price.
            </p>
        </div>
        <div>
            <h3>total.vi</h3>
            <p>This vi has three input variables: size, discount, and count. The vi should output the total price which is the multiply of size, discount, and item count. However, the cake shop has a special "buy two get one free" discount. Thus, for every three cakes, the third cake would be free. So three cakes only charge the price of two, four cakes charge three, five cakes charge four, six cakes charge four, and so on. Round the price to nearest integer.
            </p>
        </div>
    </div>
</body>