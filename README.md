make: This will build the binary file    <br/>
make run arg=<args>: This will compile the neuralnet.c file in the src directory and run the resulting binary file with the argument specified by arg. It will also generate a plot using gnuplot.  <br/>
make clean: This will remove all the object files in the lib directory   <br/>





# neural-network-from-scratch-in-c  <br/>
I implemented Neural Network from scratch in c programming.  <br/>
I implemented toy neural network in c . with following parameters  <br/>
1st argument: number of layers including output layer eg: 3 in case 2 hidden 1 output layer <br/>
2nd argument : number of neurons in each layer in list format  <br/>
Eg: 10, 10, 2   <br/>
3rd argument :activation function choice <br/>
Eg:
1 for sigmoid   <br/>
2 for tanh     <br/>
3 for relu     <br/>
4th argument is number of epochs to run eg: 1000   <br/>
5th argument: learning rate e.g 0.1    <br/>
Argument output: fun sigmoid, layers 10,2, output softmax   <br/>
<br/>
![image](https://user-images.githubusercontent.com/107786677/225321646-63dbd21f-c0a5-43c2-998f-c7c44abcfabc.png) <br/>
For argument: tanh epochs 1500 layer 10, 2 learning rate 0.1  <br/>
![image](https://user-images.githubusercontent.com/107786677/225321916-95bcb409-c33b-4ee2-abe9-fdfd917240ea.png)  <br/>
The loss function for stipper for tan h function accuracy also high <br/>
final test accuracy 95.209581 percent <br/>
![image](https://user-images.githubusercontent.com/107786677/225322059-2bce417f-f76d-441a-8837-7226bb5b24b1.png) <br/> <br/>
Loss value for rely function not giving output as expected there might be error in                                              <br/>                 
implementation but, learning is also slow <br/>
Final test accuracy <br/>
final test accuracy 60.479042 percent <br/>
Sklearn implementation <br/>
Relu 1500 epochs sgd Gives 95.1048951048951% accuracy <br/>
Sigmoid 1500 epochs sgd gives 90.83916083916084 %accuracy <br/>
Tanh 1500 epochs sgd gives 95.804195804195 % accuracy <br/>
Gradient vanishing problem occurs for sigmoid and tanh function: <br/>
It is because the sigmoid function range is 0 to 1 but its derivative range is 0.25 hence we <br/>
reduce hence we keep losing the range that we operate hence we face improper learning <br/>
rate <br/>
Slow convergence or increase in the loss function <br/>
Here I tried to implement the lost gradient descent problem <br/>
These are specifications for the arguments <br/>
3 layers 10,20,2 activation tanh function epochs 1000 learning rate 0.1 <br/>
![image](https://user-images.githubusercontent.com/107786677/225322197-267952b0-422a-4558-adaf-7dde547a1bd9.png) <br/>
Here as we can see for 3 layers <br/>
Implementation works for sigmoid function and tanh function but still fails to get good <br/>
learning rate of relu function. Problem faced in assignments is mostly incorrect <br/>
implementation of mathematics I stripped down some requirements to get a working <br/>
Network. I tested the same network on another multiclass dataset it works correctly                                             <br/>
 <br/>
