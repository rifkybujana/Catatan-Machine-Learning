# Linear Regression 

### **Definisi**
Salah satu tipe <ins>[[Regression]]</ins> dimana terjadi interpolasi garis lurus pada data
![[LinearRegression.png]]

### **Hipotesis**
*see : <ins>[[Hipotesis]]</ins>*

$\large{h_\theta = \theta_0 + \theta_1x + \theta_2x + ...}$ <br>

### **Tujuan**
Memilih $\theta(\theta_0, \theta_1, \theta_2, ...)$ sehingga $h_\theta(x)$ mendekati nilai $y$ pada training <br>

### **Cost Function**
*see : <ins>[[Cost Function]]</ins>*
*Squared Error Cost Function:*

$\LARGE {J(\theta) = \frac{1}{2m} \sum\limits_{i=1}^{m}(h_\theta(x_i)-y_i)^2}$ 

*Keterangan:*
$m$ = banyak data
$h_\theta$ = hipotesis
$y_i$ = $y$ dari training data
$J(\theta)$ = cost function

*Plotting cost function pada $J(\theta_1)$*
![[CostFunction1.png]]
*Plotting cost function pada $J(\theta_0, \theta_1)$*
![[CostFunction2.png]]

### **Gradient Descent** 
*see : <ins> [[Gradient Descent]]</ins>*

Memiliki tujuan untuk memperkecil nilai $J(\theta)$

*Rumus: *
$\large{\text{Repeat until convergence \{}}$

$\LARGE{\hspace{10mm} \theta_j \coloneqq \theta_j-\alpha \frac{\partial}{\partial \theta_j} J(\theta)}$
$\large{\text{\}}}$

Jika dijabarkan untuk semua $\theta$ maka 
$\large\theta_0=\theta_0-\alpha\frac{1}{m}(\sum\limits_{i=1}^{m}(h_\theta(x)-y_i))x_{i_0}$

$\large\theta_1=\theta_1-\alpha\frac{1}{m}(\sum\limits_{i=1}^{m}(h_\theta(x)-y_i))x_{i_1}$

$...$



*Keterangan : *
$\alpha$ = <ins>[[Learning rate]]</ins>
$\theta_j$ = Parameter theta indeks j
$\frac{\partial}{\partial\theta_j} J(\theta)$ = <ins>[[Turunan parsial]]</ins> fungsi J terhadap theta indeks j
$x_{i_n}$ = $x$ baris ke i, <ins>[[feature]]</ins> ke n


