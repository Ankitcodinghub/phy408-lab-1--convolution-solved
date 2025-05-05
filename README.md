# phy408-lab-1--convolution-solved
**TO GET THIS SOLUTION VISIT:** [Phy408 Lab 1- Convolution Solved](https://www.ankitcodinghub.com/product/phy408-lab-1-convolution-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;100503&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Phy408 Lab 1- Convolution Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
1 A Discrete Convolution Program

WriteadiscreteconvolutionfunctionmyConvthatconvolvestwoarrays{fi,i=0,…,Nf −1}and {wj, j = 0, . . . , Nw − 1} to obtain an output time series {gn}. For simplicity, assume a fixed sampling interval ∆ = 1, and further, that f and w are 0 outside of their sampled regions.

<ol>
<li>How long is {gn}? In other words, how many non-zero points can it have? Justify your answer.</li>
<li>Please copy and paste your function g = myConv(f, w) to the PDF report.</li>
<li>Provideatesttoconvinceyourself(andme)thatyourfunctionagreeswithnumpy.convolve. For example, generate two random timeseries f, w with Nf = 50, Nw = 100, drawing each element from U[0, 1], and plot the difference between your function’s output and numpy’s.Include the code for your test in the PDF report.</li>
<li>Compare the speed of your myConv function to the NumPy function. Provide a plot of thecomparison, and include your python code in the PDF report. Is your function faster or slower than the NumPy function? Can you suggest why that is the case?</li>
</ol>
Hint: For the speed test part, make up your own fi and wj time series, and for simplicity, study the cases of Nf = Nw = 10, 100, 1000, 10000. To accurately time each computation of the convolution function, import the time module and place calls to time.time around your code:

<pre>import time
t1 = time.time()
g = myConv(f, w)
t2 = time.time()
print(t2-t1)
</pre>
Alternatively, use the timeit module: import timeit

<pre>print(timeit.timeit('g = myConv(f, w)', number=10000))
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
2 Simple Physical System: RL Circuit Response

Consider a simple physical system consisting of a resistor (with resistance R) and an inductor (with inductance L) in series. We apply an input voltage a(t) across the pair in series, and measure the output voltage b(t) across the inductor alone. For this linear system,

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
<div class="column">
Take advantage of your myConv function, or the NumPy built-in function convolve, and writeyourownPythonfunctionV_out = RLresponse(R,L,V_in,dt)totakeaninputseries Vin sampled at ∆ = dt, and calculate the output series Vout sampled by the same dt. Please paste your Python function here. (Hint: here ∆ may not be 1, so remember to build the multiplication of ∆ into your convolution function.)

3. Using R = 850Ω, L = 2H, and sampling period dt = 0.20 ms, test your RL-response function with {Hn} series (discretized H(t)) as input, and plot the output time series (as circles) on top of the theoretical curve S(t) given by part 1 (as a solid line). Repeat this for {Dn} (discretized δ(t)) and R(t). Make the time range of the plots 0 to at least 20 ms. Please list your Python code here.

Convolution of Synthetic Seismograms (5 pts)

</div>
</div>
<div class="layoutArea">
<div class="column">
<ol>
<li>Showanalyticallythatitsstepresponse(i.e.,theb(t)weobtainwhentheinputvoltagea(t)= H(t), the Heaviside function) is given byS(t) = e−Rt/L H(t),

and its impulse response (i.e., the output voltage b(t) when a(t) = δ(t)) is given by

R(t) = δ(t) − RL e−Rt/L H(t).

Hint: Construct and solve the ODE relating the voltages under consideration. Consider the

two b(t) choices to derive S(t) and R(t). Formulas d H(t) = δ(t) and δ(t) f (t) = δ(t) f (0)

may help.
</li>
<li>Discretize the impulse response R(t) function, realizing that H(t) should be discretized as</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
and δ(t) should be discretized as

</div>
<div class="column">
H = [0.5,1,1,…],

D = [1/dt,0,0,…].

</div>
</div>
<div class="layoutArea">
<div class="column">
Numerical simulations of seismic wave propagation can now be routinely done for global and regional earthquakes. For a recent southern Pakistan earthquake (Jan 18, 2011, 20:23:33 UTC), raw vertical synthetic seismogram (i.e., displacement field simulated at a seismic station) for station RAYN (Ar Rayn, Saudi Arabia) is provided (RAYN.II.LHZ.sem). A common practice in seismology is to convolve synthetic seismograms with a Gaussian function

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
<div class="layoutArea">
<div class="column">
dt

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
g(t) = √ 1 e−(t/tH )2 πtH

to reflect either the time duration of the event or the accuracy of the numerical simulation.

<ol>
<li>Provide two plots. Plot 1: the raw synthetic seismogram for station RAYN between 0 and 800 seconds. Plot 2: Gaussian functions with half duration tH = 10 sec and tH = 20 sec (include a legend). For the gaussians, use the same timestep dt as the seismogram data.</li>
<li>Use numpy’s convolve function to convolve the raw timeseries with a Gaussian function (both tH = 10 and tH = 20 cases). Plot the raw data and the two convolved time series between 0 and 800 seconds on the same graph (include a legend) and comment on your results.</li>
</ol>
Hints

<ul>
<li>The raw synthetics RAYN.II.LHZ.sem is given as a text file with two columns: time in sec- onds and displacement in meters.</li>
<li>Gaussian functions quickly decay to zero beyond [−3tH,3tH], therefore it is sufficient to sample g(t) within this interval.</li>
<li>Use mode=’same’ when calling numpy convolve to truncate the convolution to the max of the supplied arrays (i.e. length of the raw timeseries in our case). This is convenient, since we want to compare the convolution output to the original timeseries. Alternatively, use the default mode (‘full’) and truncate the output manually.</li>
<li>As a check for part 2, ensure that your convolved timeseries is aligned with (or “overlaps”) the raw data timeseries.</li>
</ul>
</div>
</div>
</div>
