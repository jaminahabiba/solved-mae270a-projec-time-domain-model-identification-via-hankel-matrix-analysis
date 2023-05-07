Download Link: https://assignmentchef.com/product/solved-mae270a-projec-time-domain-model-identification-via-hankel-matrix-analysis
<br>
<h2></h2>

Consider a multi-input/multi-output, discrete-time linear system with <em>m </em>outputs and <em>q </em>inputs,

<strong>x</strong><em>k</em>+1 = <em>A</em><strong>x</strong><em>k </em>+ <em>B</em><strong>u</strong><em>k</em>

<h3>y<em><sub>k </sub></em>= <em>C</em>x<em><sub>k</sub></em></h3>

where the state dimension is <em>n<sub>s </sub></em>so <em>A </em>∈ <strong>R</strong><em><sup>n</sup></em><em><sup>s</sup></em>×<em><sup>n</sup></em><em><sup>s</sup></em>, <em>B </em>∈ <strong>R</strong><em><sup>n</sup></em><em><sup>s</sup></em>×<em><sup>q </sup></em>and <em>C </em>∈ <strong>R</strong><em><sup>m</sup></em>×<em><sup>n</sup></em><em><sup>s</sup></em>. It is assumed the feedthrough matrix <em>D </em>∈ <strong>R</strong><em><sup>m</sup></em>×<em><sup>q </sup></em>is zero. We will assume the state-space matrices have real elements. The <em>r</em>th column of the <em>pulse response </em>sequence {<em>h<sub>k</sub></em>}, where <em>h<sub>k </sub></em>∈ <strong>R</strong><em><sup>m</sup></em>×<em><sup>q</sup></em>, is obtained when <strong>x</strong><sub>0 </sub>= 0 and the input is given by the sequence in which the <em>r</em>th element of <strong>u</strong><sub>0 </sub>is 1 and all other elements are zero, and then the subsequent input samples are all zero (the “0” index indicates <em>t </em>= 0),

0



…

0<sub></sub>

<strong>u</strong>0 = 1<em>, </em>(<strong>u</strong>0)<em>r </em>= 1

0<sub></sub>

…



0 <strong>u</strong><em><sub>k </sub></em>= 0<em>, k </em>= 1<em>,</em>2<em>,</em>3<em>,…</em>

The pulse response is the discrete-time analog of the impulse response of a continuous-time system. It is straightforward to show <em>h</em><sub>0 </sub>= 0<em>, h<sub>k </sub></em>= <em>CA<sup>k</sup></em><sup>−1</sup><em>B, k </em>= 1<em>,</em>2<em>,</em>3<em>,…</em>

<table width="624">

 <tbody>

  <tr>

   <td width="319">{<em>u</em><sub>1</sub><em>,u</em><sub>2</sub><em>,…,u</em><sub>2<em>n</em></sub>−1} terms in the pulse response,</td>

   <td width="31"> </td>

   <td width="258"> </td>

   <td width="15"> </td>

  </tr>

  <tr>

   <td width="319"><em>h</em>1 <em>h</em>2 <em>h</em>3  2 <em>h</em>3 <em>h</em>4 <em>h </em><em>H<sub>n </sub></em>= <em>h</em>3              <em>h</em>4               <em>h</em>5<sup> </sup>…         …           … <em>h</em><em>n </em><em>h</em><em>n</em>+1 <em>h</em><em>n</em>+2</td>

   <td width="31">·········…···</td>

   <td width="258"><em>h<sub>n </sub></em><em>h</em><em>n</em>+1 <em>h</em><em>n</em>+2 ∈ <strong>R</strong><em>mn</em>×<em>nq</em><em>.</em>.<sup>.</sup>. <sub></sub><em>h</em>2<em>n</em>−1</td>

   <td width="15">(1)</td>

  </tr>

 </tbody>

</table>

The pulse response sequence can be organized into an <em>mn </em>× <em>nq </em>Hankel matrix, denoted <em>H<sub>n</sub></em>, by using the

A distinguishing feature of the Hankel matrix is that the elements of each anti-diagonal block are the same. By virtue of it’s definition, the Hankel matrix can be expressed as the following product,

<em>H<sub>n </sub></em>= O<em>n</em>C<em>n</em><em>,</em>

where you will recognize the observability and controllability matrices,

<em>.</em>

Next, we make the following assumption: rank O<em>n </em>= <em>n<sub>s </sub></em>and rank C<em>n </em>= <em>n<sub>s</sub></em>. In other words, O<em>n </em>and C<em>n </em>are <em>full rank </em>and in this case

rank <em>H<sub>n </sub></em>= <em>n<sub>s</sub>,</em>

that is, the state dimension is equal to the rank of the Hankel matrix constructed from the pulse response. This assumption on the rank not only requires that enough points be available so that the column and row dimensions of <em>H<sub>n </sub></em>are no less than <em>n<sub>s</sub></em>, but it also requires that certain “structural” properties of the system be satisfied –these details are discussed in the notes under the subjects of observability and controllability. If the state-space system undergoes a change of coordinates using <em>T </em>∈ <strong>R</strong><em><sup>n</sup></em><em><sup>s</sup></em>×<em><sup>n</sup></em><em><sup>s</sup></em>, det<em>T </em>= 06 ,

<strong>z</strong><em>k</em>+1 = <em>T</em>−1<em>AT</em><strong>z</strong><em>k </em>+ <em>T</em>−1<em>B</em><strong>u</strong><em>k</em>

<strong>y</strong><em><sub>k </sub></em>= <em>CT</em><strong>z</strong><em><sub>k</sub></em>

Note that O<em>n </em>and C<em>n </em>transform to

O<em>n </em>→7   O˜<em>n </em>= O<em>n</em><em>T,         </em>C<em>n </em>7→ C˜<em>n </em>= <em>T</em>−1C<em>n</em>

Of course, the impulse response remains the same and so does the Hankel matrix <em>H<sub>n </sub></em>= O<em>n</em>C<em>n </em>= O˜<em><sub>n</sub></em>C˜<em><sub>n</sub></em>.

Now consider the situation in which the pulse response samples are provided. In this case, <em>H<sub>n </sub></em>can be formed from {<em>h<sub>k</sub></em>}, <em>k </em>= 0<em>,</em>1<em>,</em>2<em>,… </em>, according to (1). Compute an SVD of <em>H<sub>n</sub></em>,

<em>,</em>

where <em>U</em><sub>1 </sub>∈ <strong>R</strong><em><sup>mn</sup></em>×<em><sup>n</sup></em><em><sup>s</sup></em>, Σ<em><sub>n</sub></em><em><sub>s </sub></em>∈ <strong>R</strong><em><sup>n</sup></em><em><sup>s</sup></em>×<em><sup>n</sup></em><em><sup>s</sup></em>, <em>V</em><sub>1 </sub>∈ <strong>R</strong><em><sup>nq</sup></em>×<em><sup>n</sup></em><em><sup>s</sup></em>. O<em>n </em>and C<em>n </em>can be determined from the SVD, however, the factorization is not unique since it is possible to group terms into O<em>n </em>or into C<em>n</em>, for example,

O<em>n </em>= <em>U</em>1 and C<em>n </em>= Σ<em>n</em><em>s</em><em>V</em>1<em>T</em><em>, </em>or O<em>n </em>= <em>U</em>1Σ<em>n</em><em>s </em>and C<em>n </em>= <em>V</em>1<em>T</em><em>,</em>

or<em>, </em>or<em>, </em>for any invertible <em>W.</em>

A specific choice of factorization just corresponds to a <em>specific choice of coordinates </em>in which the state-space matrices are to be expressed. Whatever factorization is used, <em>C </em>is selected to be the first <em>m </em>rows of O<em>n </em>and <em>B </em>is selected to be first <em>q </em>columns of C<em>n</em>. To recover <em>A</em>, a new Hankel matrix is computed,

<em>.</em>

Once O<em>n </em>and C<em>n </em>have been determined from <em>H<sub>n </sub></em>using your desired factorization, a left inverse of O<em>n</em>, denoted

†

O<em>n</em>, and a right inverse of C<em>n</em>, denoted C<em>n</em>†, are used to compute <em>A </em>in the same coordinates as <em>C </em>and <em>B</em>,

<em>A </em>= O<em>n</em><sup>†</sup><em>H</em>˜<em><sub>n</sub></em>C<em>n</em><sup>†</sup><em>.</em>

Although left and right inverses are not unique (unless the matrix is, in fact, invertible, in which case the left and right inverses are equal to the usual inverse) the product O<em>n</em>†<em><sup>H</sup></em><sup>˜</sup><em><sub>n</sub></em>C<em>n</em>† is always unique so it does not matter which left or right inverse is used. The SVD of <em>H<sub>n </sub></em>conveniently allows specification of left and right inverses using the matrices from the decomposition. For example, if O<em>n </em>= <em>U</em><sub>1 </sub>and, then and.

In practice, the Hankel matrix is full rank so the “best” way to recover a model is to analyze the singular values of <em>H<sub>n </sub></em>and make a judgement on a suitable model order. For example, if there is a notable “jump” in the singular values (like in Fig. 3), then a sensible approach is to retain the largest singular values and truncate those after the “jump”. Thus, although <em>H<sub>n </sub></em>is full rank, it is approximated by a rank <em>n<sub>s </sub></em>matrix, where <em>n<sub>s </sub></em>is the <em>selected </em>model order. In other words, <em>n<sub>s </sub></em>is not <em>a priori </em>specified –it is determined from analysis of the data, and once determined, <em>H<sub>n </sub></em>is replaced by the “optimal” rank <em>n<sub>s </sub></em>approximation

<sup></sup><em>σ</em><sub>1         </sub>0      ···         0 <sup></sup>

<sub></sub>0      <em>σ</em>2                                 

<em>, </em>where Σ<em>n</em><em>s </em>=  …                 …         

0                         <em>σ</em><em>n<sub>s</sub></em>

where <em>U</em><sub>1 </sub>and <em>V</em><sub>1 </sub>represent the first <em>n<sub>s </sub></em>columns of <em>U </em>and <em>V </em>, respectively (where <em>U </em>and <em>V </em>are the unitary matrices from an SVD of <em>H<sub>n</sub></em>). Lastly, often times an analytical model of the system is available and will provide insight into an expected model order. It is important to reconcile what an analytical model yields versus what the test data suggests since resolving a discrepancy can often lead to greater insight into the system.

<h2>1.2        A note on the Gramian relations</h2>

Recall the observability and controllability gramians using the first <em>n </em>samples of the impulse response are defined as

If we make the following choices for O<em>n </em>and C<em>n</em>,

then the gramians are <em>balanced</em>, in other words, <em>G<sub>o</sub></em>(<em>n</em>) = <em>G<sub>c</sub></em>(<em>n</em>) = Σ<em><sub>n</sub></em><em><sub>s</sub></em>, because

Now if the system is asymptotically stable we can take the limit <em>p </em>→ ∞, then

(2)

(3)

and these gramians satisfy the corresponding discrete-time Lyapunov equations,

<em>A<sup>T</sup>G<sub>o</sub></em>(∞)<em>A </em>− <em>G<sub>o</sub></em>(∞) = −<em>C<sup>T</sup>C</em>

<em>AG<sub>c</sub></em>(∞)<em>A<sup>T </sup></em>− <em>G<sub>c</sub></em>(∞) = −<em>BB<sup>T</sup>.</em>

It’s not possible to let <em><sup>p </sup></em>→ ∞ since only a finite amount is data is collected, however, if the Hankel matrix is constructed from essentially the entire transient pulse response data record, then for all practical purposes

<em>G<sub>o</sub></em>(<em>n</em>) ≈ <em>G<sub>o</sub></em>(∞) and <em>G<sub>c</sub></em>(<em>n</em>) ≈ <em>G<sub>c</sub></em>(∞)<em>.</em>

Thus, these coordinates represent the traditional “balanced realization.” It is not necessary to decompose the

Hankel matrices so that balanced coordinates are used. Recall that

<h2>1.3        Impulse response data</h2>

Data sets can be downloaded from the course website. The data sequences are associated with a sample period of <em>t<sub>s </sub></em>= 1<em>/</em>40 second. You need to write up a report based on the modeling and analysis of a two-input/two-system that produced this input-output data. The data sets you need are called u1_impulse.mat and u2_impulse.mat. The following code loads the pulse response data and graphs it. Note that only one input channel is “on” in each data set. In this problem, <em>m </em>= 2 (two outputs) and <em>q </em>= 2 (two inputs). The state dimension is not known, though, with the objective being the determination of a state-space discrete-time system that can replicate the observed data. Note that we seek an asymptotically stable model because the impulse response data decays to zero. Also note that when using data sets from physical systems that rank <em>H<sub>n </sub></em>= <em>n </em>because inevitably there is some noise in the measurement data and furthermore the system may be nonlinear even though it can be well-approximated with a linear model. Thus, it appears that you would need an <em>n</em>-dimensional system to model the data, but a lower rank approximation almost always produces a “better” model. For example, asymptotic stability of the identified model is not explicitly enforced and using high model dimensions can actually produce unstable models.

clear close all load u1_impulse.mat

y11 = u1_impulse.Y(3).Data; y21 = u1_impulse.Y(4).Data; u1 = u1_impulse.Y(1).Data; %%% note that the pulse magnitude is 5 [m,mi] = max(u1&gt;0); %%% find index where pulse occurs load u2_impulse.mat

y12 = u2_impulse.Y(3).Data; y22 = u2_impulse.Y(4).Data; u2 = u2_impulse.Y(2).Data;

%%% remove any offsets in output data using data prior to pulse application y11 = y11 – mean(y11([1:mi-1])); y12 = y12 – mean(y12([1:mi-1])); y21 = y21 – mean(y21([1:mi-1])); y22 = y22 – mean(y22([1:mi-1]));

%%% rescale IO data so that impulse input has magnitude 1 y11 = y11/max(u1); y12 = y12/max(u2); y21 = y21/max(u1); y22 = y22/max(u2); u1 = u1/max(u1); u2 = u2/max(u2);

ts = 1/40; %%%% sample period

N = length(y11); %%%% length of data sets t = [0:N-1]*ts – 1;

figure(1); subplot(311) plot(t,u1,’b*’,’LineWidth’,2) ylabel(’$u_1$ (volts)’,’FontSize’,14,’Interpreter’,’Latex’); grid on axis([-0.2 2 -0.1 1.1])

subplot(312) plot(t,y11,’r*’,’LineWidth’,2) ylabel(’$y_1$ (volts)’,’FontSize’,14,’Interpreter’,’Latex’); grid on axis([-0.2 2 -0.1 0.1])

subplot(313) plot(t,y21,’r*’,’LineWidth’,2) ylabel(’$y_2$ (volts)’,’FontSize’,14,’Interpreter’,’Latex’); grid on xlabel(’second’,’FontSize’,14) set(gca,’FontSize’,14) axis([-0.2 2 -0.1 0.1])

figure(2); subplot(311) plot(t,u2,’b*’,’LineWidth’,2) ylabel(’$u_2$ (volts)’,’FontSize’,14,’Interpreter’,’Latex’); grid on axis([-0.2 2 -0.1 1.1])

subplot(312) plot(t,y12,’r*’,’LineWidth’,2) ylabel(’$y_1$ (volts)’,’FontSize’,14,’Interpreter’,’Latex’); grid on axis([-0.2 2 -0.1 0.1])

subplot(313)

plot(t,y22,’r*’,’LineWidth’,2)

ylabel(’$y_2$ (volts)’,’FontSize’,14,’Interpreter’,’Latex’); grid on xlabel(’second’,’FontSize’,14) set(gca,’FontSize’,14) axis([-0.2 2 -0.1 0.1])

This Matlab code produces Figs. 1 and 2. At the <em>k</em>th sample time, the <em>y</em><sub>1 </sub>and <em>y</em><sub>2 </sub>values from Fig. 1 form the first column of <em>h<sub>k </sub></em>∈ <strong>R</strong><sup>2×2</sup>, and the <em>y</em><sub>1 </sub>and <em>y</em><sub>2 </sub>values from Fig. 2 form the second column of <em>h<sub>k</sub></em>. The singular values of <em>H<sub>n</sub></em>, <em>n </em>∈ {20<em>,</em>40<em>,</em>80}, are shown in Fig. 3 where there appear to be seven dominant singular values regardless of the dimension of <em>H<sub>n </sub></em>(assuming enough points are used). This suggests that a reasonable initial choice of model order is <em>n<sub>s </sub></em>= 7. You will select a handful of model orders and derive the corresponding state-space models from the Hankel matrix factorization and then compare your models in a few different ways.

<h3>Task #1: Model identification</h3>

Complete the following:

<strong>Figure 1: </strong>System response when <em>u</em><sub>1 </sub>is a unit impulse and <em>u</em><sub>2 </sub>is zero.

<strong>Figure 2: </strong>System response when <em>u</em><sub>2 </sub>is a unit impulse and <em>u</em><sub>1 </sub>is zero.

<strong>Figure 3: </strong>Singular values of <em>H</em><sub>20 </sub>(blue), <em>H</em><sub>40 </sub>(red) and <em>H</em><sub>80 </sub>(green). Only the first 40 singular values are shown for each case.

<ol>

 <li>Construct <em>H</em><sub>100 </sub>and graph the singular values. Compute models from <em>H</em><sub>100 </sub>with the following state dimensions: <em>n<sub>s </sub></em>∈ {6<em>,</em>7<em>,</em>10<em>,</em>20}. There is no need to print out the state-space matrices since you will compute the model properties below. Calculate the max(abs(eig(A))) to confirm that all models are asymptotically stable.</li>

 <li>Simulate the impulse response of each model and compare it to the measurement data. Use a separate figure for each case (model response versus data). Which model order has an inferior reproduction of the pulse response data? The remaining models are essentially indistinguishable, though, and could be used as a valid model for the system.</li>

 <li>Another way to compare the model to the data is to compare the model frequency response to the empirical frequency response obtained from the pulse response data. The model frequency response is given by</li>

</ol>

<em>C</em>(<em>e</em><em>jωt</em><em>s</em><em>I </em>− <em>A</em>)−1<em>B </em>+ <em>D,</em>

where <em>t<sub>s </sub></em>= 1<em>/</em>40 is the sample period in seconds. The frequency <em>ω </em>is in the interval [0<em>,ω<sub>nyq</sub></em>], where <em>ω<sub>nyq </sub></em>is the Nyquist frequency (equal to one half the sampling frequency, in other words, <em>ω<sub>nyq </sub></em>= 20 hertz). Note that when evaluating the formula, <em>ω </em>should have units of radians-per-second. At each frequency, the frequency response is a 2 × 2 matrix with complex-valued elements. Plot the magnitude and phase of the frequency response of each model with <em>n<sub>s </sub></em>∈ {6<em>,</em>7<em>,</em>10<em>,</em>20}. There will be a total of eight figures because each scalar input-output channel has a magnitude and phase plot (all magnitudes of the (1,1) channel will be compared in a single figure, all phases of the (1,1) channel will be compared in a single figure, and so forth). Don’t forget to label your figures.

<ol start="4">

 <li>The pulse response data can be used to directly estimate the frequency response without the need for a parametric model. For example, let y11 be the impulse response data associated with output <em>y</em><sub>1 </sub>due to a unit pulse applied by input <em>u</em><sub>1 </sub>(where the data sequence is u1). Then, the frequency response associated with this channel can be estimated using the following code:</li>

</ol>

y11f = fft(y11)./fft(u1); N = length(y11f);

om = [0:N-1]/(ts*N); %%%% frequency vector in hertz

Estimate the empirical frequency response magnitude and phase and <em>overlay </em>these results on the model plots from the previous part. Thus, in each of the eight figures generated in the previous part, you will have 5 traces: 4 from the models and one from the empirical frequency response estimate. You should observe that three of the models match up very well with the empirical frequency response results.

<h3>Task #2: Transmission zeros of the MIMO model and zeros of each channel</h3>

Consider the model in which <em>n<sub>s </sub></em>= 7 for this task. This model provides a very accurate reproduction of the pulse response data and, furthermore, the model frequency response is very close to the empirical frequency response. You can confirm the <em>normal rank </em>of

is 9, that is, rank <em>S</em>(<em>α</em>) = 9 for almost all <em>α </em>∈ <strong>C</strong>. A transmission zero of the system occurs at <em>z </em>∈ <strong>C </strong>when rank <em>S</em>(<em>z</em>) <em>&lt; </em>9. In this case, there exist non-zero vectors <strong>c </strong>∈ <strong>C</strong><sup>7 </sup>and <strong>w </strong>∈ <strong>C</strong><sup>2 </sup>such that

Let the input be <strong>u</strong><em><sub>k </sub></em>= <strong>w</strong><em>z<sup>k</sup></em>, <em>k </em>= 0<em>,</em>1<em>,</em>2<em>,… </em>. The state vector <strong>x</strong><em><sub>k </sub></em>= <strong>c</strong><em>z<sup>k </sup></em>satisfies the difference equation with this input because

<strong>c</strong><em>.</em>

<strong>x</strong><em>k                   </em><strong>u</strong><em>k</em>

Furthermore, the output is zero for all samples because

<strong>y</strong><em><sub>k </sub></em><em>.</em>

The zeros can be computed from a generalized eigenvalue problem,

<em>.</em>

See the Matlab eig command for more information on solving this generalized eigenvalue problem. Answer the following:

<ol>

 <li>Show that there are five <em>finite </em>transmission zeros of the <em>n<sub>s </sub></em>= 7 model, with the remaining four zeros given as “inf.” The inf zeros can be ignored. Label the zeros from largest to smallest magnitude. Note |<em>z</em><sub>1</sub>| <em>&gt; </em>1 is called an unstable zero because the input it generates is unbounded, however, |<em>z<sub>p</sub></em>| <em>&lt; </em>1, <em>p </em>= 2<em>,</em>3<em>,</em>4<em>,</em>5, are asymptotically stable zeros because the inputs they generate decay to zero, i.e. .</li>

 <li>Graph the eigenvalues and transmission zeros of the <em>n<sub>s </sub></em>= 7 model in the complex plane. Draw a circle of radius 1 (use the Matlab command axis square so the aspect ratio is one-to-one) and note that if your model is asymptotically stable (it should be) then the eigenvalues will lie within the unit circle. Denote the eigenvalues with an “x” and the transmission zeros with a “o.”</li>

 <li>A discrete-time eigenvalue <em>λ<sub>d </sub></em>can be converted into its “equivalent” continuous-time eigenvalues according to <em>λ<sub>d </sub></em>= <em>e<sup>λ</sup></em><em><sup>c</sup></em><em><sup>t</sup></em><em><sup>s</sup></em>, where <em>λ<sub>c </sub></em>is the continuous-time eigenvalue. Note that imaginary part of <em>λ<sub>c </sub></em>is not uniquely defined, so just choose the smallest value for the imaginary part of <em>λ<sub>c </sub></em>(this choice is justified as long as there is no aliasing of resonant frequencies during the data collection). From the set of <em>λ<sub>c</sub></em>, how many damped oscillators are in your model and what are their approximate natural frequencies? How do the frequencies compare with certain features in frequency response graphs?</li>

 <li>For the <em>n<sub>s </sub></em>= 7 model, graph the eigenvalues and transmission zeros calculated for <em>each individual channel</em>. Note that the eigenvalues will be the same in all cases so the transfer functions in each channel are different because their zeros are different. Reconcile the channel frequency responses with the pole-zero plots, i.e. the presence or lack of the resonances and so forth. Furthermore, treating each channel as a separate system, what are its Hankel singular values? You should observe that each channel, considered in isolation, can actually be described with a lower order model whose dimension is consistent with the near pole-zero cancellations that you observe in each channel.</li>

 <li>Now return to the Hankel matrix and select <em>n<sub>s </sub></em>= 8. This model is over-parameterized in some sense because its pulse response and frequency response are essentially identical to those associated with the <em>n<sub>s </sub></em>= 7 Create another pole-zero plot for each channel and show that the added pole is accompanied by zero in close proximity and that this occurs for all channels. This creates essentially a pole-zero cancellation in each channel so that the “extra” state dimension in the <em>n<sub>s </sub></em>= 8 case does not have much impact on the input-output properties of the system compared to the <em>n<sub>s </sub></em>= 7 model.</li>

</ol>

<h3>Task #3: Block diagram from analysis of individual channels</h3>

From the analysis of the two input-two output system, there appear to be two oscillators in the system. Furthermore, there are three poles on the positive real axis (near 0.8). These poles correspond to low-pass filters. The poles of each oscillator are distinct (despite the fact that they are quite close) so give each complex conjugate pair of oscillator poles a distinct label like “OSC1” and “OSC2”. Also label the three distinct real poles as “LP1”, “LP2” and “LP3”. Now based on which poles are not canceled by zeros in the individual channels (from the previous Task results), draw a block diagram showing how OSC1, OSC2, LP1, LP2 and LP3 are “connected” to form the two input-two output system. Can you uniquely determine the topology? If not, what parts cannot be resolved? Finally, some channels have a zero at <em>s </em>= 1 –this zero can be combined with one of the low-pass poles to create a high-pass filter. Which one of the low-pass poles (LP1 and/or LP2 and/or LP3?) can be paired with this zero to make the high-pass filter and how are the effects of the high-pass filter evident in the frequency response graphs?

<h1>2          Correlation functions</h1>

A pulse input to a system is not always ideal in order to determine its impulse response because disturbances and measurement noise also contribute to the observed outputs, and because of limitations on how large the input magnitude can be, it may not be possible to increase the pulse height to a level where the system’s response is dominated by the effect of the pulse input. Thus, it is advantageous to use inputs which are persistent since it is possible to transfer more energy to the system when limits on the input magnitude are present, as is always the case in any real test environment. A persistent input which is quite useful in this regard is “white noise.” Before defining white noise, the auto- and cross-correlation functions are defined for discrete-time persistent signals <strong>u</strong><em><sub>k </sub></em>∈ <strong>R</strong><em><sup>n </sup></em>and <strong>y</strong><em><sub>k </sub></em>∈ <strong>R</strong><em><sup>m</sup></em>,

Auto-correlation of <strong>u </strong>: <strong>R</strong><em><sup>n</sup></em><sup>×<em>n                                                                               </em></sup>(4)

Auto-correlation of <strong>y </strong>: <em>,                                                </em>(5)

Cross-correlation : <em>.                                                 </em>(6)

The index <em>k </em>is called the “lag index” which corresponds to the time lag <em>t<sub>s</sub>k</em>, where <em>t<sub>s </sub></em>is the sample period for the data. It is assumed the correlation functions are independent of the time origin, i.e. the assumption that <strong>u </strong>and <strong>y </strong>are stationary. The input signal <strong>u </strong>is “zero mean, unit variance white noise” when

<em> .                                                                                   </em>(7)

In this case, different scalar channels of <strong>u </strong>are uncorrelated for all lag factors <em>k </em>and, furthermore, each scalar channel has only non-zero correlation with itself when <em>k </em>= 0.

Suppose <strong>u </strong>and <strong>y </strong>are the input-output sequences associated with an asymptotically stable linear time-invariant system, then, <strong>u </strong>and <strong>y </strong>are related via convolution,

∞                                      ∞

<strong>y</strong><em>k </em>= X <em>h</em><em>k</em>−<em>l</em><strong>u</strong><em>l </em>= X <em>h</em><em>l</em><strong>u</strong><em>k</em>−<em>l</em>

<em>l</em>=−∞                                 <em>l</em>=−∞

where <em>h<sub>k </sub></em>is the system’s pulse response function. In this case, the cross-correlation reduces to

This result demonstrates that a “virtual” test can be conducted: if input <strong>u </strong>produces output <strong>y</strong>, then input <em>R</em><strong><sub>uu </sub></strong>produces output <em>R</em><strong><sub>yu</sub></strong>. Importantly, if <strong>u </strong>is zero-mean, unit variance white noise, then <em>R</em><strong><sub>uu </sub></strong>is given by (7) and so <em>R</em><strong><sub>yu</sub></strong>[<em>k</em>] = <em>h<sub>k</sub></em>.

<h2>Task #4: Impulse response identification from white noise inputs</h2>

Download the data set u_rand.mat. This data set consists of 10 minutes of input-output data. You can assign labels to the different elements of the inputs and outputs as follows:

load u_rand.mat y1 = u_rand.Y(3).Data; y2 = u_rand.Y(4).Data; u1 = u_rand.Y(1).Data; u2 = u_rand.Y(2).Data; ts = 1/40; N = length(y1); t = [0:N-1]*ts – 1;

The sample period remains <em>t<sub>s </sub></em>= 1<em>/</em>40 second for this data. Its necessary to assess the statistical properties of the input signals. We can establish that each channel is zero-mean, uncorrelated white noise. Answer the following,

<ol>

 <li>Verify that each input sequence is approximately zero mean.</li>

 <li>Determine and graph estimates of the four entries of <em>R</em><strong><sub>uu </sub></strong>for indices <em>k </em>∈ [−200<em>,</em>200]. Plot the entries versus lag factor <em>τ </em>∈ [−5<em>,</em>5] second (which corresponds to the indices <em>k </em>∈ [−200<em>,</em>200]).</li>

 <li>Show that</li>

</ol>

Thus, the variance of each input channel is 4, not 1.

<ol start="4">

 <li>Estimate <em>R</em><strong><sub>yu</sub></strong>[<em>k</em>] for <em>τ </em>∈ [−0<em>.</em>2<em>,</em>2] second and then graph the first column of <em>R</em><strong><sub>yu </sub></strong>normalized by the variance of the first channel of <strong>u </strong>and graph the second column of <em>R</em><strong><sub>yu </sub></strong>normalized by the variance of the second channel of <strong>u</strong>. Compare your results to the experimental impulse response obtained from the pulse response experiments -the results should be close!</li>

</ol>

<h1>3          System norms</h1>

Just norms were defined for vectors and matrices, it is possible to define norms for systems and in this case, the input “vectors” are actually drawn from some class of signals. Some system norms are induced norms, and others are not. One major difference between signal and system norms compared to norms on finite dimensional vector spaces is that on finite dimensional vector spaces (including matrices) all norms are <em>equivalent </em>in the sense that a vector that is small in one norm will also be small in another norm. This does not generalize to norms on infinite dimensional vector spaces, i.e. linear spaces of signals and systems.

<h2>3.1        H2 norm</h2>

The H<sub>2 </sub>norm of a linear, time-invariant system, is defined as the square root of the integral of the square of the Frobenious norm of the system’s impulse response. In other words, if “<em>P</em>” represents a continuous-time LTI system, then

Z ∞

k<em>P</em>k<sup>2</sup><sub>H</sub>2 =            k<em>h</em>(<em>t</em>)k<sup>2</sup><em><sub>F </sub></em><em>dt,        h </em>= continuous-time impulse response

−∞

when the integral exists, otherwise the norm is infinite. If the system is causal, then the lower limit of integration can be set to 0. Necessary and sufficient conditions for the integral to exist when <em>P </em>is a continuous-time system (as opposed to a discrete-time system) are that <em>P </em>is asymptotically stable <em>and </em>the direct feedthrough term <em>D </em>in the state-space realization must be zero. The latter condition is needed because if <em>D </em>6= 0 then impulses appear in <em>h</em>, and impulses do not have finite energy in the continuous-time case.

For causal discrete-time systems, the expression is modified accordingly,

∞ k<em>P</em>k<sup>2</sup><sub>H</sub>2 = <sup>X</sup>k<em>h<sub>k</sub></em>k<sup>2</sup><em><sub>F </sub></em><em>,        h<sub>k </sub></em>= discrete-time pulse response<em>.            </em>(8)

<em>k</em>=0

In the discrete-time case <em>D </em>need not be zero, however, we will assume <em>D </em>= 0 here since it simplifies the formula (also, the systems you have identified have the property <em>D </em>= 0). Note that (8) can be manipulated as follows, assuming the system is causal, asymptotically stable, and has the state-space realization <strong>x</strong><em><sub>k</sub></em><sub>+1 </sub>= <em>A</em><strong>x</strong><em><sub>k </sub></em>+ <em>B</em><strong>u</strong><em><sub>k</sub></em>, <strong>y</strong><em><sub>k </sub></em>= <em>C</em><strong>x</strong><em><sub>k</sub></em>,

(9)

or, alternatively,

(10)

where <em>G<sub>o</sub></em>(∞) and <em>G<sub>c</sub></em>(∞) are the observability and controllability gramians that can be computed from the Lyapunov equations (2), (3).

The most relevant interpretation of the H<sub>2 </sub>norm from an engineering perspective is as follows: it is the root-mean-square (RMS) measurement of the output <strong>y </strong>when each channel of the input <strong>u </strong>is a zero-mean, white signal with autocorrelation

function

The RMS value of a discrete-time signal <strong>v </strong>is defined as

<em>.                                                                          </em>(11)

Despite the usage of the norm notation, the RMS value of a signal is <em>not </em>a norm (“transient” non-zero signals have zero RMS value, however, the other norm properties are satisfied). Nevertheless, it is a very useful measure of a signal’s “size”, especially when the signal is “random.”

To make the connection between the RMS value of the output <strong>y </strong>and the H<sub>2 </sub>norm definition, note that k<strong>y</strong>k<sub>R</sub><em><sub>MS </sub></em>can also be expressed as

<em>.</em>

Since <em>R</em><strong><sub>yy</sub></strong>[0] has special significance, compute it:

!

This result is general, however, when <strong>u </strong>is zero-mean, unit variance white noise, in other words

then <em>R</em><strong><sub>yy</sub></strong>[0] reduces to

∞

<em>R</em><strong>yy</strong>[0] = X <em>h</em><em>q</em><em>h</em><em>Tq </em><em>.</em>

<em>q</em>=−∞

The RMS value of the output is

k<strong>y</strong>k<sup>2</sup>RMS = tr <em>R</em><strong><sub>yy</sub></strong>[0]

!

<h3>Task #5: H2 norm analysis of identified model</h3>

You will use the u_rand.mat data set for this analysis, too. You have already verified

<em> .</em>

This shows the input channels are not unit variance, however, because the variances are both approximately 4, you can scale the input and output data by a factor 2 so that each input channel now has unit variance. You also showed that the individual channels of <strong>u </strong>have no correlation with each other. Compute and compare the following:

<ol>

 <li>the RMS value of the scaled output data <strong>y</strong>,</li>

 <li>k<em>P</em>k<sub>H</sub>2 , where <em>P </em>is your 7-state model derived from the Hankel matrix analysis; use both (9) and (10) for the system norm calculation,</li>

 <li>approximate k<em>P</em>k<sub>H</sub>2 from (8) using the experimental pulse response data only (no model).</li>

</ol>

These calculations should yield essentially the same values.

<h2>3.2        H∞ norm</h2>

The H<sub>2 </sub>norm of a system is of great importance in control systems design because a typical objective is to design the controller so that the H<sub>2 </sub>norm of certain closed-loop input-output channels in minimized (say, from some force disturbances that are modeled as broadband white noise inputs to the motion of a vibration-sensitive instrument; in this case it is very natural to consider the H<sub>2 </sub>norm of those IO channels as something to be minimized with feedback). Although the H<sub>2 </sub>can be interpreted as an induced norm, the signal norms for the inputs and outputs are different: “energy” norm for the inputs and the maximum absolute value in time norm for the outputs. The H<sub>2 </sub>norm does not satisfy the submultiplicative property. In other words, there are examples in which two systems, denoted <em>P</em><sub>1 </sub>and <em>P</em><sub>2</sub>, have the property k<em>P</em><sub>2</sub>·<em>P</em><sub>1</sub><sup>k</sup><sub>H</sub>2 <em>&gt; </em>k<em>P</em><sub>2</sub><sup>k</sup><sub>H</sub>2k<em>P</em><sub>1</sub><sup>k</sup><sub>H</sub>2 , where <em>P</em><sub>2 </sub>·<em>P</em><sub>1 </sub>denotes the series connection of these systems. This property makes the H<sub>2 </sub>norm unsuitable for addressing another critical aspect of control systems design, namely, the robustness of the controller to perturbations of the plant dynamics.

The H<sub>∞ </sub>norm of an asymptotically stable linear system <em>P </em>is defined as

<em>,                                                                               </em>(12)

where <em>P</em>(<em>jω</em>) represents the system’s frequency response function and <em>σ </em>represents the maximum singular value. The “sup” operation over frequency returns the <em>least upper bound </em>of <em>σ</em>(<em>P</em>(<em>jω</em>)). In many cases, “sup” can be replaced with “max”. If the system is not asymptotically stable then k<em>P</em><sup>k</sup><sub>H∞ </sub>= ∞.

It is easily seen from its definition that the H<sub>∞ </sub>norm is submultiplicative. Furthermore, it can be shown that the H<sub>∞ </sub>norm is an induced norm on an appropriate space of input and output functions so the submultiplicative property follows from this as well. There are several reasons why the H<sub>∞ </sub>norm is useful in the robustness analysis of feedback systems. First, the fact that this system norm has strong connections with the frequency response makes it convenient to use in modeling the deviations of the system from a “nominal” model. For example, you may test a system under a variety of operating conditions and find that you can associate multiple frequency responses with the system –it just depends on what conditions the system is operating under. One modeling approach is to define a nominal model and a permissible level of deviation from the nominal model, quantified by the H<sub>∞ </sub>norm, so that all empirical frequency responses are included in the <em>set of models </em>generated by the nominal model along with a permissible deviation. Thus, a model of the following form may be generated:

<em>P</em>(<em>jω</em>) = (<em>I </em>+ <em>w</em>(<em>jω</em>)∆(<em>jω</em>))<em>P</em><sub>0</sub>(<em>jω</em>)<em>.                                                                          </em>(13)

In this example the “true” plant is described as a multiplicative perturbation of a nominal plant <em>P</em><sub>0</sub>. The perturbation is an asymptotically stable, but unknown, system with k∆k<sub>H∞ </sub><em>&lt; </em>1. The scalar weight <em>w </em>is what controls the “size” of the perturbation: if |<em>w</em>(<em>jω</em>)| <em>&lt;&lt; </em>1 at certain frequencies, then <em>P </em>≈ <em>P</em><sub>0 </sub>at those frequencies; on the other hand, if |<em>w</em>(<em>jω</em>)| <em>&gt;&gt; </em>1 at other frequencies, then we are admitting we really don’t know the “true” plant model at those frequencies despite the fact that the nominal model <em>P</em><sub>0 </sub>is well-defined. This is a very natural way to model a system and will be appreciated by those who have some test and measurement experience, especially with regard to empirical frequency response estimates. A second point demonstrating the usefulness of H<sub>∞ </sub>norm comes from the fact that a controller, denoted <em>G</em>, will stabilize all plants <em>P </em>of the form (13) if and only if k<em>w</em>(<em>I </em>+ <em>P</em><sub>0</sub><em>G</em>)<sup>−1</sup><sup>k</sup><sub>H∞ </sub>≤ 1, which may be interpreted as a bound on the frequency response of a weighted closed-loop transfer function obtained with the nominal model. This conclusion is possible only because the H<sub>∞ </sub>norm is submultiplicative. This is the subject of robust control and is covered in more detail in courses like MAE273.

<strong>State-space computation of </strong>k<em>P</em>k<sub>H∞ </sub><strong>–continuous-time case</strong>

The definition of the H<sub>∞ </sub>norm suggests that a search over frequency can be performed. This is possible, however a more elegant way uses a state-space model of the system. First, consider an asymptotically stable continuous-time system “<em>P</em>” given by <strong>x</strong>˙ = <em>A</em><strong>x </strong>+ <em>B</em><strong>u</strong><em>, </em><strong>y </strong>= <em>C</em><strong>x </strong>+ <em>D</em><strong>u</strong>. The frequency response function is <em>P</em>(<em>jω</em>) = <em>C</em>(<em>jωI </em>− <em>A</em>)<sup>−1</sup><em>B </em>+ <em>D </em>and by definition

<em>.</em>

Note that and so the state-space system that produces this expression for its frequency response is given by <strong>z</strong>˙ = −<em>A</em><sup>∗</sup><strong>z </strong>+ <em>C</em><sup>∗</sup><strong>u</strong>˜<em>, </em><strong>y</strong>˜ = −<em>B</em><sup>∗</sup><strong>z </strong>+ <em>D</em><sup>∗</sup><strong>u</strong>˜. The frequency response product is created by a series connection of these two systems (the physical system <em>P </em>and the non-physical one), so a state-space realization can be determined for the series connection as follows:

<strong>u</strong>

(14)

<strong>y</strong>˜ <strong>u</strong>

The frequency response from <strong>u </strong>to <strong>y</strong>˜ produces (<em>P</em>(<em>jω</em>))<sup>∗</sup><em>P</em>(<em>jω</em>). Let the “system” from <strong>u </strong>to <strong>y</strong>˜ be denoted <em>L</em>. We also introduce a positive parameter <em>γ </em>whose role will be clarified in a moment. We multiply each output channel of <strong>y</strong>˜ by 1<em>/γ</em><sup>2</sup>. For a fixed <em>γ</em>, suppose at some frequency <em>ω</em><sub>0 </sub>the largest eigenvalue associated with the frequency response of  is equal to 1, and has corresponding eigenvector <strong>v</strong>. Recall that the frequency response of <em>L </em>is hermitian at each frequency so all eigenvalues of <em>L</em>(<em>jω</em>) are real. In other words, suppose, and hence<strong>v</strong>, for some <strong>v </strong>6= 0. We surmise

Importantly, in this case there exists the following input-output relationship,

<h2>y˜(<em>t</em>) = cos(<em>!</em><sub>0</sub><em>t</em>)vv</h2>

Since there is a forced solution in which the input is equal to the output, we can “close the loop” and such a solution will still exist for the closed-loop system,

<h1>y˜(<em>t</em>) = cos(<em>!</em><sub>0</sub><em>t</em>)v</h1>

Thus, the closed-loop system must have an eigenvalue at <em>jω</em><sub>0 </sub>since a sustained oscillation is possible in the absence of external excitation. Conversely, if the closed-loop system has an eigenvalue <em>jω</em><sub>0</sub>, then it can be shown that the open loop system frequency response must have an eigenvalue of 1. The closed-loop “<em>A</em>” matrix, denoted <em>A<sub>clp</sub></em>(<em>γ</em>), is a function of <em>γ </em>and is computed by setting <strong>u</strong><strong>y</strong>˜ in the state-space equations (14). The first expression to manipulate is the output equation,

<em>γ</em><sup>2</sup><strong>u</strong><em> D</em><sup>∗</sup><em>D</em><strong>u</strong>

|{z} <strong>y</strong>˜

where <em>D<sub>γ </sub></em>is defined as  and is assumed to be invertible (we will show why <em>D<sub>γ </sub></em>can always be assumed to be invertible). Now substitute this expression for <strong>u </strong>into the differential equation part of the state-space discription,

<strong>u</strong>

In conclusion, k<em>P</em>k            ≥ <em>γ </em>⇐⇒ there exists a purely imaginary eigenvalue(s) of <em>A<sub>clp</sub></em>(<em>γ</em>)

H∞

or equivalently, k<em>P</em>k          <em>&lt; γ </em>⇐⇒ there exists no purely imaginary eigenvalues of <em>A<sub>clp</sub></em>(<em>γ</em>)

H∞

Thus, instead of searching over frequency for the largest singular value of <em>P</em>(<em>jω</em>), we search over <em>γ </em>and determine whether

<em>A<sub>clp </sub></em>has imaginary eigenvalues. A bisection procedure on <em>γ </em>can compute k<em>P</em>k                       to arbitrary accuracy.

H∞

A final word is necessary on the assumed invertibility of <em>D<sub>γ</sub></em>. Since lim<em><sub>ω</sub></em><sub>→∞ </sub><em>P</em>(<em>jω</em>) = <em>D</em>, then a <em>lower bound </em>for k<em>P</em>k

H∞ is <em>σ</em>(<em>D</em>). In other words, in the bisection search over <em>γ </em>we can always take <em>γ &gt; σ</em>(<em>D</em>) which guarantees invertibility of <em>D<sub>γ</sub></em>.

<strong>State-space computation of </strong>k<em>P</em>k<sub>H∞ </sub><strong>–discrete-time case</strong>

The frequency response associated with the discrete-time system <strong>x</strong><em><sub>k</sub></em><sub>+1 </sub>= <em>A</em><strong>x</strong><em><sub>k </sub></em>+ <em>B</em><strong>u</strong><em><sub>k</sub>, </em><strong>y</strong><em><sub>k </sub></em>= <em>C</em><strong>x</strong><em><sub>k </sub></em>+ <em>D</em><strong>u</strong><em><sub>k</sub></em>, is

and the H<sub>∞ </sub>norm of the system is defined as

<em>.</em>

The problem with extending the continuous-time analysis to the discrete-time case is due to the fact that it is not immediately apparent how to manipulate  into another discrete-time system with an equivalent frequency response (the problem is how to deal with <em>e</em><sup>−<em>jωt</em></sup><em><sup>s</sup></em>) so another approach will be taken.

Consider a partitioned matrix <em>M </em>in which <em>M</em><sub>11 </sub>∈ <strong>C</strong><em><sup>m</sup></em><sup>×<em>p</em></sup>, <em>M</em><sub>21 </sub>∈ <strong>C</strong><em><sup>n</sup></em><sup>×<em>p</em></sup>, <em>M</em><sub>12 </sub>∈ <strong>C</strong><em><sup>m</sup></em><sup>×<em>n </em></sup>and <em>M</em><sub>22 </sub>∈ <strong>C</strong><em><sup>n</sup></em><sup>×<em>n</em></sup>. Also consider <em>Q </em>∈ <strong>C</strong><em><sup>n</sup></em><sup>×<em>n</em></sup>. Imagine “connecting” the matrices in the following manner:

where the vectors have the following dimensions <strong>y </strong>∈ <strong>C</strong><em><sup>m</sup></em>, <strong>u </strong>∈ <strong>C</strong><em><sup>p</sup></em>, <strong>z </strong>∈ <strong>C</strong><em><sup>n </sup></em>and <strong>w </strong>∈ <strong>C</strong><em><sup>n</sup></em>. This relationship reduces to

<strong>y</strong><em>,                                                                </em>(15)

where it is assumed that <em>I </em>− <em>M</em><sub>22</sub><em>Q </em>is invertible.                               The frequency response function for the continuous-time system <strong>x</strong>˙ =

<em>A</em><strong>x </strong>+ <em>B</em><strong>u</strong><em>, </em><strong>y </strong>= <em>C</em><strong>x </strong>+ <em>D</em><strong>u </strong>is

where upon comparison with (15) we observe that the frequency response can be interpreted in this framework by selecting <em>M</em><sub>11 </sub>= <em>D</em>, <em>M</em><sub>12 </sub>= <em>C</em>, <em>M</em><sub>21 </sub>= <em>B</em>, <em>M</em><sub>22 </sub>= <em>A</em>, and <em>Q </em><sup>= </sup><em><sub>jω</sub></em><u><sup>1 </sup></u><em>I</em>. Similarly, the frequency response function associated with the discrete-time system <strong>x</strong><em><sub>k</sub></em><sub>+1 </sub>= <em>A</em><strong>x</strong><em><sub>k </sub></em>+ <em>B</em><strong>u</strong><em><sub>k</sub>, </em><strong>y </strong>= <em>C</em><strong>x</strong><em><sub>k </sub></em>+ <em>D</em><strong>u</strong><em><sub>k </sub></em>can be computed by setting <em>M</em><sub>11 </sub>= <em>D</em>, <em>M</em><sub>12 </sub>= <em>C</em>, <em>M</em><sub>21 </sub>= <em>B</em>,

<em>M</em><sub>22 </sub>= <em>A</em>, and <em>Q </em>= <em><sub>e</sub></em><em>jωt</em><sup>1 </sup><em><sub>s </sub></em><em>I</em>. Thus, the frequency responses can be pictorially represented,

The frequency response of the discrete-time system can be related to the frequency response of an “equivalent” continuoustime system by noting that for any <em>ω </em>∈ [0<em>,ω<sub>nyq</sub></em>) (note that <em>ω<sub>nyq </sub></em>is excluded), <em>e<sup>jωt</sup></em><em><sup>s </sup></em>is uniquely related to <em>ν </em>∈ <strong>R </strong>according to the bilinear transformation,

(16)

but since 1<em>/e<sup>jωt</sup></em><em><sup>s </sup></em>appears in the diagram, we need to derive a relation between it and 1<em>/jν</em>,

(17)

The continuous-time system has no direct physical meaning -it is merely constructed so that it’s frequency response function at any given “frequency” <em>ν </em>has a unique match with the physical discrete-time system’s frequency response.

The “equivalent” continuous-time system can be determined by noting that (17) also has the following pictorial representation,

If we insert the right-hand diagram into the diagram for the discrete-time frequency response, it can be rearranged as shown on the right by eliminating the internal <strong>z </strong>and <strong>w </strong>signals,

where the “continuous-time” state-space matrices are computed to be

(18)

Thus, in order to compute the H<sub>∞ </sub>norm for the discrete-time system, we “convert” the state-space matrices into the continuoustime form (18) and then apply the bisection search procedure over <em>γ </em>using <em>A<sub>clp</sub></em>(<em>γ</em>) formed from the matrices in (18). If H<sub>∞ </sub>norm is <em>γ</em><sub>0 </sub>then <em>A<sub>clp</sub></em>(<em>γ</em><sub>0</sub>) has one or more eigenvalues that are purely imaginary. The frequency at which the maximum is achieved, however, needs to be determined so let <em>ν</em><sub>0 </sub>be the imaginary part of one of the purely imaginary eigenvalues of <em>A<sub>clp</sub></em>(<em>γ</em><sub>0</sub>). Compute the corresponding <em>ω</em><sub>0 </sub>from (16) to determine the frequency at which the largest singular value of the frequency response occurs. The only frequency not covered by the search procedure is <em>ω </em>= <em>ω<sub>nyq </sub></em>so the discrete-time frequency response is just checked separately for this case.

<h2>Task #6: H∞ norm analysis of identified model</h2>

Complete the following:

<ol>

 <li>Write a Matlab function that accepts as inputs the state-space matrices of a continuous-time system, upper and lower limits for the <em>γ </em>search, and a tolerance, and then returns the H<sub>∞ </sub>norm of the system computed to within the specified tolerance, and the approximate frequency at which the maximum gain is achieved.</li>

 <li>Write a Matlab function that accepts as inputs the state-space matrices of a discrete-time system, upper and lower limits for the <em>γ </em>search, a tolerance, and the sample period <em>t<sub>s </sub></em>associated with the system, and then returns the H<sub>∞ </sub>norm of the system computed to within the specified tolerance, and the approximate frequency at which the maximum gain is achieved. Note that this Matlab function can call the Matlab function you wrote for the continuous-time case.</li>

 <li>Compute the H<sub>∞ </sub>norm of your identified discrete-time model using the Matlab functions, including the frequency at which it is achieved.</li>

 <li>Compute the discrete-time frequency response of the identified model on a frequency grid in the interval [0<em>,ω<sub>nyq</sub></em>] and then plot the singular values of the frequency response on this frequency grid. Overlay on top of the singular values, the singular values that you compute from the empirical frequency response data. You should observe that the model singular values are very close to the empirical singular values and that the H<sub>∞ </sub>norm computed from the model locates the magnitude and corresponding frequency where the maximum singular value achieves its largest value.</li>

</ol>