# geog0111-coursework-part-b-p0-solved
**TO GET THIS SOLUTION VISIT:** [Geog0111 Coursework Part B P0 Solved](https://www.ankitcodinghub.com/product/geog0111-p0-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;124614&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Geog0111 Coursework Part B P0 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (2 votes)    </div>
    </div>
Geog0111 Scientific Computing

Coursework (Assessed Practical) Part B

Instructions and marking grids

URL: https://github.com/UCL-EO/geog0111

1. IntroductionAssignment Project Exam Help

1.1 Task overview

The main coding exercises involve building a set of Python functions, then running these, passing data between the functions, and visualising results. a set of You must provide and run the functions that you should develop in a Jupyter notebook, as well as showing results in the notebook.

1.2 Submission

You must develop and run the codes in a single Jupyter notebook, and submit the work in a single notebook as a PDF file. As usual with coursework, you must attach a cover page declaration.

2. Background

2.1 Model background

In this part of your assessment you will be using, calibrating and validating such a model that relates temperature and snow cover in the catchment to river flow.

We will use the model to describe the streamflow at the Del Norte measurement station, just on the edge of the catchment. You will use environmental (temperature) data and snow cover observations to drive the model. You will perform calibration and testing by comparing model output with observed streamflow data.

Assignment Project Exam Help

Figure 1. Del Norte station

Further general information is available from various websites, including NOAA. You can visualise the site Del Norte 2E here. This is the site we will be using for river discharge data.

Figure 2. River near Del Norte station

2.3 Model

2.3.1 Model basics

We will build a simple mass balance model that is capable of predicting daily streamflow at some catchment location for given temperature and catchment snow cover. This defines the purpose of our model (how we will use it) and describes the model output (daily streamflow QdN[t] at some catchment location) and drivers (temperature T[t] and catchment snow cover p[t]):

We will need 2 dynamic datasets to run the model, given for samples in time t:

• T[t]: mean temperature (C) at the Del Norte monitoring station for each day of the year • p[t]: Catchment snow cover (proportion) and one dataset to calibrate and test the model, for samples in time:

• QdN[t]: stream flow data for each in units of megalitres/day (ML/day i.e. units of 1000000 litres a day) at the del Norte monitoring station.

As we have noted, you will be running, calibrating and testing a mass-balance snowmelt model in the Rio Grande Headwaters in Colorado, USA. In such a model, we keep track of the mass of some parameter of interest, here the snow water-equivalent (SWE), the amount of water in the snowpack for the catchment. We assume the reservoir of water is directly proportional to snow cover p[t]at time t so:

SWE[t] = kAssignment Project Exam Help1 p[t] (1)

with k1 a constant of proportionality relating to snow depth and density.

We need a mechanism in the model that converts from SWE[t] to flow dQ[t], the water flowing into the system from the snowpack at time t. We can consider this as:

dQ[t] = k2 m[t] SWE[t]

= k1 k2 m[t] p[t]

= k m[t] p[t] (2)

where dQ[t]is the amount of water flowing into the catchment at time t, m[t] is a proportion of the snowpack assumed to melt at time t, and k2 a constant of proportionality relating to the proportion of the SWE that is available to be converted. We combine the constants of proportionality so k=k1 k2.

You can imagine the snow water equivalent SWE[t]as a quantity of snow in a bucket observed at time t, and there being some proportion k2 of this that has the potential to melt and become water dQ[t]. You can think of there being a tap or valve that releases that water into another bucket at time t, with m[t] (between 0 and 1) being a measure of how much that valve is open or closed. The main control on this tap is temperature at time t, T[t]. In the simplest form, this would be a switch, so setting m to 0 when flow is off (too cold to melt) and m to 1 when flow is on (hot enough to melt). Practically, we model the rate of release of water from the snowpack as a logistic function of temperature:

m[t] = expit([T[t]-T0]/xp) (3)

where expit the logistic function that we have previously used in phenology modelling. This is a form of ‘soft’ switch between the two states (still with melting, m=0, and melting m=1). If the temperature is very much less than the threshold T0, it will remain frozen. If it is very much greater than T0, there will be an amount proportionate to SWE[t] flowing into the system on day t.

Figure 3. melt rate m[t] for varying value of parameter T0

The parameter, xp (C) increases the slope of the function at T=T0 with increasing xp. So it can be used to modify the ‘speed’ of action, or ‘sensitivity’ of the soft switch. We will use a default value of xp=1. It is likely to have only a minor impact on the modelling results so we can use this assumed value of the parameter. By keeping this parameter at a fixed value, we can simplify the problem you need to solve to one involving a single parameter to model the water release. We assume that T0 can be calibrated for a given catchment.

Assignment Project Exam Help

So:

dQ[t] = k p[t] expit((T[t]-T0)/xp) (4)

This is driven by T[t] and p[t] and controlled by parameters T0 and to a lesser extent xp. If we normalise our measures, i.e. dQ[t]/dQmax and QdN[t]/QdNmax, with dQmax and QdNmax, being the maximum values of Q[t] and QdN[t] respectively, then we can compare the quantity of melt water at time t with the measured flow at the monitoring station.

In the figure below, we see the normalised modelled melt water dQ[t] (scaled) that corresponds to a T0 of 9 C derived from datasets T[t] and p[t], alongside the normalised measured flow QdN[t] (scaled) at the del Norte station. dQ[t] is remarkably similar to the flow data QdN[t], but much noisier. We also see that it occurs some time before we see the water flow at the monitoring station. The reason for this is that there is a ‘network delay’ between the melt happening in the snowpack and it reaching the monitoring station. This final component of our model is a network response function (NRF) that models this delay in the routing of the melt water.

Figure 5. Available water dQ[t] for T0=9 C (green) plotted alongside measured flow (black) and driving data

2.3.3 Flow delay to the measuring stations

To be able to generate our desired model output, we now have to consider how this reservoir of water is transported to predict daily streamflow at some catchment measurement location. We do this using the concept of a Network Response Function (NRF). In this sub-model, we assume that the flow from out reservoir dQ[t] to the catchment measurement location can be characterised as a decay function after time t=0. So, some proportion of the water released is immediately transported to the station, and a lesser amount reaches the next day, and less the next day and so on. So, if we put a pulse of water into the system we would measure a simple decay function. This pulse response is the NRF.

Figure 6. Network Response Function (NRF) as a function of time to f=20 days

The NRF is effectively a one-sided smoothing filter. It imparts a delay on the signal dQ[t] and smooths it. We can use a function such as a one-sided Laplace distribution, a one-sided exponential parameterised by a rate of decay value f (days) to model the probability of water reaching the monitoring station at time t.

Q’dN[t] = dQ[t] * L1(t/f) (5)

Where Q’dN[t] is the modelled flow (we use ’for modelled flow here) output at the del Norte station, * is the convolution operator, dQ[t]is the snowmelt entering the reservoir at time t, and L1(t/f) is the NRF response, a one-sided Laplace (exponential) distribution:

L1(x) = exp[-x]/N | x &gt;= 0 (6) 0 |

with the normalisation factor:

N = S L1(x)

Figure 7. Network Response Function (NRF) as a function of time for varying f

You can think of this model as allowing the meltwater that becomes available at time t, dQ[t], to be spread out over time when it reaches the monitoring station. So, in figure 7 for f=10, around 0.09 of the melt water goes immediately to the monitoring station, then less than that the next day, and so on, until almost all of the water has reached the station after around 40 days. The ‘spread’ of this then is controlled by the parameter f. If f is increased to 20, only 0.05 of the water goes directly to the station, and it is spread out over a longer time period. So, f is characteristic of the catchment physical properties and the location of the snow sources relative to the monitoring station. We assume it to be a constant here, something that can be calibrated for the catchment and station.

2.3.4 Model

If, for the moment, we ignore the parameter xp, then we can illustrate out model as in the figure below:

Figure 8. Model description

The complete model has three parameters that control model behaviour:

• the threshold temperature T0 (C);

• the delay parameter f (days) of the Network Response Function (NRF)

• the temperature sensitivity parameter xp (C)

Summary:

You can find code implementing and running the model in notebooks/066_Part2_code.ipynb in the notes.

3. Coursework Detail

3.1 Basic requirements for this submission

In Part A of the assessment (that you have already completed part), you generated and visualised environmental datasets for daily temperature T[t] (C) and measured stream flow QdN[t] (ML/day) that we will be using in this part.

3.2 Required components

• Snow data preparation [40%]

• Model inversion [60%]

Each of these parts has multiple components.

3.2.1 Snow data preparation

The aim of this part of the work is for you to produce datasets of snow cover for the Hydrological Unit Code (HUC code) catchment 13010001 (Rio Grande headwaters in Colorado, USA) using MODIS snow cover data. You should by now have plenty of experience of accessing and using the MODIS LAI product, and we have already come across the snow product in 030_NASA_MODIS_Earthdata.

You must provide: Assignment Project Exam Help

• A function with argument year (integer) that returns a Pandas dataframe or dictionary containing keys for day of year (doy) and daily catchment mean snow cover p[doy] for HUC catchment 13010001.

of the year, averaged (mean) over HUC catchment 13010001.

• You must do the gap-filling for each pixel in the catchment along the time-axis. You should then take the mean of the gap-filled data over the catchment.

• You can optionally also cache this information in a file, and read the data from that file. If you use a cache, you must specify a keyword to switch on- or off- the use of the cached file .

• Do not make use of global variables to pass information to a function: you must pass all information required by a function via arguments and/or keywords.

3.2.2 Model inversion

You should now have access to datasets for

• T : mean temperature (C) at the Del Norte monitoring station for each day of the year, read from a csv file. • Q : stream flow data (ML/day) for each day of the year, read from a csv file.

• p : Catchment snow cover (proportion) returned by the function developed above .

You will need to use a LUT inversion to provide a calibration and validation of the model described above. You should be familiar with this approach from the material covered in the course and should use numpy to implement it.

You must provide:

• A calibration function with argument year (integer) that returns a dictionary or Pandas df containing the calibrated model parameters and the goodness of fit metric at the LUT minimum in calibration, along with appropriate datasets that you can use to visualise and verify the calibration results.

• It should use a LUT approach to calibrate the 2-parameter snowmelt model presented above for year.

• It should read the datasets T and Q from their CSV files for year, performing any necessary filtering or gapfilling (e.g. replace NaN values).

• It should get the snow cover dataset p for year from the function developed for snow data preparation above.

• A validation function with arguments year (integer) and the output of the calibration function that returns a dictionary or Pandas df containing the goodness of fit metric achieved in validation and other appropriate datasets that you can use to visualise the validation results.

• It should read the datasets T and Q from their CSV files for year, performing any necessary filtering or gapfilling (e.g. replace NaN values).

• It should get the snow cover dataset p for year from the function developed for snow data preparation above.

• It should compare the model-predicted and measured values of Q and provide appropriate summary statistics of the goodness of fit for the validation.

• You must provide appropriate visualization of the measured and modelled data sets.

• You must present the model parameters derived from the calibration.

• You must present a short paragraph of text describing the calibration and validation results.

• Optionally, you might also illustrate the LUT operation.

3.2.3 Advice on development of the snow cover dataset

sds = [‘NDSI_Snow_Cover’] product = ‘MOD10A1’ tile = [‘h09v05’]

warp_args = {

‘dstNodata’ : 255,

‘format’ : ‘MEM’,

‘cropToCutline’ : True,

‘cutlineWhere’ : f”HUC=13010001″,

‘cutlineDSName’ : ‘data/Hydrologic_Units/HUC_Polygons.shp’

}

That said, the first time you go through the coursework, we recommend you do use a high-level function such as this to make sure that you can complete this part of the coursework. If can later return and develop your own code, in which case you will have a previous result you can check yours against. You will get more credit for codes that show more coding skills that just calling these high level codes. You should only submit one version of the codes you develop.

You might find additional visualisations of interest, such as the space-time plots we did for the LAI time series visualisations.

4. Coursework Submission

You must develop and run the codes in a single Jupyter notebook, and submit the work in a single notebook as a PDF file.
