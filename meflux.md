---

layout: page
title: Mesoscale Enhancement 
math_engine: mathjax

---

<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

<h3>About Heat Fluxes</h3>

Near the air-sea interface, two processes that transfer heat between the ocean and atmosphere are:

1. **Sensible Heat Flux**: A difference between the air temperature and sea surface temperature (SST) leads to a transfer of energy by conduction 
2. **Latent Heat Flux**: A difference between the humidity of the air and the saturation humidity of a parcel of air at SST leads to a net moisture transfer. The phase transition between liquid and gas carries latent heat with it. 

Both of these processes are enhanced by a shear across the air-sea interface (which is primarily a function of surface winds, as ocean currents are weak). The relationships between surface winds and these heat fluxs is complicated, but can be approximated by a "bulk formula." For example, the bulk formula of latent heat flux $$F_q$$ is:

$$F_q \equiv C_q U(q - q_s)$$ 

In the tropics, heat fluxes between the ocean and atmosphere play a crucial role on virtually every timescale. On meso- and synoptic timescales, these fluxes add heat and moisture to the boundary layer, fueling deep convection and convective systems (including tropical cyclones). On climatological timescales, these fluxes are part of a net energy budget that, in the tropics, transfers heat from the ocean into the atmosphere.

My project focused on quantifying heat flux on timescales between these two extremes, namely:
1. **Intraseasonal scales**, where we found variations in heat fluxes are determined exclusively by wind patterns (which are in turn related to the MJO). 
2. **Seasonal scales**, where we found variations in heat fluxes are determined by the migration of large-scale atmospheric features such as the ITCZ and monsoon.
3. **Interannual scales**, where we found variations in heat fluxes are determined by well-known air-sea coupled oscillations (e.g. ENSO), but that these relationships are quite spatially confined despite the global atmospheric implications of these interannual variations. 



<h3>What is Mesoscale Enhancement?</h3>

Imagine taking hourly wind measurements at a single location. Suppose that the beginning of the day, winds are steadily out of the north, but that halfway through the day, they weaken and shift to coming out of the east. How do you calculate the daily average of the windspeed at this location? There are to methods I'll consider:
1. Calculating the windspeed $$U = \sqrt{u^2 + v^2}$$ at each hour, and then averaging (called the "scalar average")
2. Calculating the daily average of $$u$$ and $$v$$, then plugging into the formula for $$U$$ above.

The vector average sounds like a more accurate average from a geometric perspective. But in reality, the scalar average gives gives the true windspeed, while the vector average returns an underestimate. This happens because, to put it simply, the formula for calculating $$U$$ is nonlinear, and thus the addition and scalar multiplication involved in the operation of calculating a daily average does not commute with the operation of calculating the scalar windspeed. 

Mesoscale Enhancement is given by:

$$ME_q \equiv \left<C_q U\Delta q\right> - C_q(V,\left<q\right>,\ldots)V\left<\Delta q\right>$$

<h3>Calculating Latent Heat Flux</h3>

For this project, I used data from the Global Tropical Moored Buoy Array (GTMBA), managed by the Pacific Marine Environmental Laboratory (PMEL). GTMBA consists of three sub-arrays: TAO/TRITON in the Pacific Ocean, PIRATA in the Atlantic, and RAMA in the Indian Ocean. Combined, there have been 126 buoys deployed and/or currently in use, shown in the following map:

\*Map

with some locations having data available in the 1990s or earlier. but this extensive coverage still yielded a median of 11\*? years of data per buoy, on average.

<h3>About this Project</h3>

I completed this project through an internship as part of the <a href="https://www.noaa.gov/office-education/hollings-scholarship">Hollings Scholarship</a>. The Hollings Scholarship enables students in the geosciences and related fields to complete internships with NOAA employees, and I am very grateful for the opportunity this provided!

My internship was conducted under the mentorship of <a href="https://pmel.noaa.gov/scientist/dr-michael-james-mcphaden">Michael McPhaden</a>, at PMEL. Mike is the director of the GTMBA, and I am very thankful for his guidance on this project and beyond!

<a href="https://www.pmel.noaa.gov/gtmba/">Learn more about the GTMBA.</a>
