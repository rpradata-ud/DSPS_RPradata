Part 1.

"Bad" plot:

<img width="422" alt="Screen Shot 2023-11-18 at 2 00 14 PM" src="https://github.com/rpradata-ud/DSPS_RPradata/assets/143296355/fba07525-6aed-49b9-94a4-ca8f7b261668">

The figure above is from Kaib & Volk, 2022 (link: https://arxiv.org/pdf/2206.00010.pdf). It intends, for illustrative purposes, to show the distribution of particle semimajor axis, eccentricity, and inclination, from an Oort cloud formulation simulation after a 4Gyr evolution. The article describes that from the graphs, one can see that the scattered disk generally has perihelia between ~ 30-40 AU and inclination below ~ 45 degrees before semimajor axis ~ 10^3 AU. However, I think this is hard to eyeball from the graph because there are too many points overplotted, especially in the bottom panel (for inclination). Furthermore, it is hard to comprehend the distribution after ~ 10^3 because of this reason. Setting the “alpha” plotting parameter can help show the “thickness”/“density” of certain populated regions. One could also use a scatter contour or a density histogram to illustrate the distribution.

"Good" plot: 

<img width="526" alt="Screen Shot 2023-11-25 at 9 37 30 PM" src="https://github.com/rpradata-ud/DSPS_RPradata/assets/143296355/79ad9104-9501-48b7-98f5-b21c343b7673">

The figure above is from Sánchez-Sierras et al., 2023 (link: https://arxiv.org/pdf/2311.12933.pdf). It shows certain line profiles of certain epochs pertaining a black hole transient GRS 1915+105. I think this plot is good because it has a neat and readable layout. The left and right sides are clearly seperated as the different Epochs, and horizontally, one can see the line profiles for each corresponding epoch. The y-axes for both left and right sides follow the same scales, which makes it easier to compare line profiles between the 2 epochs. The figure also strives to make efficient use of vertical space by only showing the x-axis labels on the far bottom plots. This way, the figure can draw the vertical dashed lines (marking the velocities) through the 3 line profiles. However, one can also point out the color choice for the dashed lines (red and green) could be modified if there is a strong intention to distinguish between the velocities. 



Part 2

Plot from my research

In my research, I am making a comparative study between solar wind data at Mercury observed by the MESSENGER spacecraft, and solar wind data at the planet, during the same time, simulated by a solar wind model (called the AWSoM). I am especially looking at the radial magnetic field component of the solar wind profile. The comparison is run using Dynamic Time Warping, due to a prior knowledge that the simulation and observation are time-shifted by varying time intervals. Hence, the points are mapped from one series to another based on the "most similar features" computed by the algorithm. The differences in magnetic field strength between these comparison points are recorded in a histogram, shown in the figures below. 

Before:

<img width="628" alt="Screen Shot 2023-11-26 at 1 22 45 PM" src="https://github.com/rpradata-ud/DSPS_RPradata/assets/143296355/8b93b23c-95ea-43bc-bf11-07e4bcd423a2">


After:

<img width="623" alt="Screen Shot 2023-11-26 at 1 21 59 PM" src="https://github.com/rpradata-ud/DSPS_RPradata/assets/143296355/06ed0024-bea8-442c-aed5-e388a0c4c924">

Fig. 1: Histogram of the differences in magnetic field strength between MESSENGER observation and simulation (observation subtracted by simulation), during a certain period of time in the year 2013. Negative differences indicate that the simulated strength is lower than observed, and vice versa for positive differences. The top panel shows before correction, and bottom shows after. The most noticeable difference between plots I made was the number of bins/bin size. In our case here, we wanted more specific information about the strength shift





top and bottom panels
figure captions specify what minus what
