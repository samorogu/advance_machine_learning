## 1.-Choose correct statements about the exploding gradient problem
* **Exploding gradient problem is easy to detect** You can actually see the loss
* ReLU nonlinearity helps with the exploding gradient problem. It helps with vanishing gradient problem
* **The reason of the exploding gradient problem in the simple RNN is the recurrent weight matrix $W$. Nonlinearities sigmoid, tanh, and ReLU does not cause the problem.** $W$ cause the vanishing or exploding gradient, and large $W$ cause exploding gradients, especially with ReLU
* The threshold for gradient clipping should be as low as possible to make the training more efficient 


## 2.-Choose correct statements about the vanishing gradient problem

* Vanishing gradient problem is easy to detect.False, It's hard to detect. convergence or vanishing gradient
* **Both nonlinearity and the recurrent weight matrix$W$ cause the vanishing gradient problem*
* **Orthogonal Initialization of the recurrent weight matrix helps with vanishing gradient problem**,
* Truncated BPTT helps with the vanishing gradient problem. False. it makes the gradient from faraway steps equal to zero. It's for exploding gradients


## 3.-Choose correct statements about this architecture


* The LSTM needs four times more parameters than the simple RNN. **True, $V$ is not just single $V$. it consists of $V_f, V_i, V_g, V_o$ ** 
* Gradients do not vanish on the way through memory cells $c$ in the LSTM with forget gate. **False ${\partial c_t \over \partial c_{t-1}} = f_t$** and forget gate may take values from 0 to 1, therefore vanishing gradient problem is still possible here and careful initialization of forget gate is needed ,
* There is a combination of the gates values which makes the LSTM completely equivalent to the simple RNN **False, The LSTM is very similar to the simple RNN when input and output gates are open and forget gate is closed. However, they are not completely equivalent because in the LSTM nonlinearity $\tilde f$ is used twice on the way between $h_{t-1}$ to $h_t$** 
* The exploding gradient problem is still possible in the LSTM on the way between $h_{t-1}$ and $h_t$ **True, Very large norm of $W$ may cause the exploding gradient problem. Therefore gradient clipping is usefull for LSTM and GRU architectures too**

## 4.-Consider the GRU architecture:
$g_t = \tilde f(V_g x_t + W_g(h_{t-1}\cdot r_t)+b_g )$
$ h_t =(1-u_t)\cdot g_t +u_t \cdot h_{t-1} $ 

* Both reset and update gates are open.
* Both reset and update gates are closed.
* **Reset gate is open and update gate is closed.**
* Update gate is open and reset gate is closed.


