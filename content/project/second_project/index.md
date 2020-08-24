---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Moho Depth Estimation in Iran through Geopotential Models and Euler Deconvolution Method"
summary: ""
authors: []
tags: [Moho Depth]
categories: []
date: 2020-01-09T15:57:19+03:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "featured.png"
  focal_point: ""
  preview_only: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
<DIV align="justify">

The Moho discontinuity is the boundary between the Earth's crust and the underlying mantle. The Moho depth in different zones of Iran has been estimated by various approaches like analysis of receiver function method according to teleseismic waves recorded in seismic stations; inversion of terrestrial gravity data and using Bouguer gravity anomaly and free air gravity anomaly; spectral correlation analysis of terrain gravity effects; thermal analysis and using geoid height; Parker-Oldenburg method; Least squares Collection. For instance, the first of crustal thickness variations have been computed from Bouguer anomaly modelling by Dehghani & Makris (1984) for the whole Iran. Based on their results, crustal thickness is 55 km beneath the main Zagros thrust, 45–48 km in eastern Iran and 35 km below the Alborz mountains. In this study, a new approach was used to estimate the Moho depth in structural zones of Iran based on geopotential models and 3D Euler Deconvolution method. The Euler Deconvolution method is a semi-automated process and supports the interpretation of magnetic field data, gravimetry data or gravity gradiometry data. It is used to estimate the location of the source of a magnetic or a gravity field anomaly. Euler Deconvolution method is not dependent on an initial depth or density limitations ([Reid et al., 1990](https://pubs.geoscienceworld.org/geophysics/article-abstract/55/1/80/72314/Magnetic-interpretation-in-three-dimensions-using?redirectedFrom=fulltext); [Mushayandebvu et al., 2001](http://geophysics.geoscienceworld.org/content/66/3/814.abstract)). Based on [Keating (1998)](http://www.google.com/url?q=http%3A%2F%2Fgeophysics.geoscienceworld.org%2Fcontent%2F63%2F5%2F1595.abstract&sa=D&sntz=1&usg=AFrqEzfb8PJ20hVRP5wTB88OJFav6RqTFA) and [Silva & Barbosa (2003)](http://geophysics.geoscienceworld.org/content/68/6/1962.abstract), this algorithm is proper to determine depth of vertical and horizontal contacts, so it is good to be used in estimating the crust-mantle boundary (Moho depth).


[Thompson (1982)](http://geophysics.geoscienceworld.org/content/47/1/31) showed that Euler's homogeneity relation could be written in the form:

</DIV>

$$(x-x_0)\frac{\partial T}{\partial x} + (y-y_0)\frac{\partial T}{\partial y} +(z-z_0)\frac{\partial T}{\partial z} = N(B-T)$$

<DIV align="justify">
Where (x<sub>0</sub>, y<sub>0</sub>, z<sub>0</sub>) is the position of a source whose total field T, is detected at (x, y, z). The total field has a regional or background value B. N is the degree of homogeneity, interpreted physically as the fall-off rate with distance and geophysically as a Structural Index (SI), Structural Index can change from 0 to 2 for gravity data. Because of high volume of data used in magnetic or gravimetric methods and lack of access to high precision and quality in overall processing of data in whole grid, Euler square window has been defined according to:
</DIV>

{{< figure src="2.jpg" title="Euler Deconvolution Algorithm" numbered="true" lightbox="true" >}}

<DIV align="justify">

The process is done inside the window and unknown parameters (B, x<sub>0</sub>, y<sub>0</sub>, z<sub>0</sub>) are calculated using least squares adjustment. This window must have two characteristics ([Barbosa et al., 1999](https://library.seg.org/doi/abs/10.1190/1.1444529)): 1. It should be large enough to incorporate substantial variation of the field and field gradient.; 2. It should be small enough not to include significant effects from multiple sources.


[Mushayandebvu et al. (2004)](https://library.seg.org/doi/abs/10.1190/1.1707069) studied influence of structural index on depth uncertainty and source position using a synthetic anomaly. Their studies show that an estimated depth for an anomaly may considerably change following structural index changes while location (or horizontal) uncertainties (X<sub>offset</sub>, Y<sub>offset</sub>) won't change much. Although it is possible to have same anomaly using two structural indices, estimating depth of each structural index will be completely different. Another important parameter is window size which influence estimated depth in each solution. Generally speaking, solutions with much bigger or much smaller depths than window size are not acceptable, in these situations the resulted source cannot fit on geometry of hypothetical model. [Reid et al. (1990)](http://geophysics.geoscienceworld.org/content/55/1/80.abstract) studied relation between anomalous depth and window size, they found out that the minimum acceptable depth is equal to window size and its maximum is about three times the window size. [Barbosa et al. (2000)](https://www.sciencedirect.com/science/article/pii/S0926985199000476) showed that it is possible to calculate (x<sub>0</sub>, y<sub>0</sub>) parameters (horizontal position of source) through selection of proper window size according to the model with no attention to N. But to calculate depth parameter (z<sub>0</sub>) which is the most important parameter in interpretation of gravity data, selection of structural index must be done precisely. Window size is a function of model depth and smaller window size provides larger errors for deeper depth because deeper masses have wider anomaly which in order to be included, the window must be wider. In simpler words, small windows deliver proper solutions for shallow anomalies while large windows provide small errors in depth estimation of deep masses.


Geopotential models provide homogeneous and uniformly accurate information on the long wavelengths of the earth's gravity field. Since these Models have long wavelengths of gravity field, they are very suitable in determining Moho depth because short and middle wavelengths are not useful in this case. Accuracy of the geopotential models are usually evaluated by comparing the geoidal heights derived from the models with those of the local GPS-Leveling stations. After comparing EIGEN-GL04C model to GPS-Leveling data, it has been chosen as the most accurate model in Iran. In this research, free air gravity anomaly from EIGEN-GL04C model (Up to degree and order of 360; Long wavelengths of gravity field) as the total field (T) and ETOPO1 Model for considering topography effect were used for estimating Moho depth.


</DIV>

{{< figure src="featured.png" title="Free air gravity anomaly resulted from EIGEN-GL04C (The Zagros Zone)" numbered="true" lightbox="true" >}}

{{< figure src="ETOPO1.png" title="Topography resulted from ETOPO1 (The Zagros Zone)" numbered="true" lightbox="true" >}}


<DIV align="justify">

A lot of research has been done about relationship between anomalous depth and spherical harmonic degree. [Bowin (1983)](https://www.tandfonline.com/doi/abs/10.1080/15210608309379476#.VAH1uHbrf1U) showed that second- and third-degree spherical harmonics are related to sources near to mantle-core boundary. Also [Hager (1984)](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/JB089iB07p06003) showed that fourth- to ninth-degree spherical harmonics are in relation with density models of subducted slab. Although it is not possible to calculate radial distribution of anomalous masses uniquely, but it is known that deeper and bigger sources produce lower degree harmonics of gravity field while higher degree harmonics are produced by shallow and smaller sources ([Jackson et al., 1991](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1365-246X.1991.tb01158.x)). According to [Bowin et al. (1986)](https://pubs.geoscienceworld.org/geophysics/article-abstract/51/1/123/72071/Depth-estimates-from-ratios-of-gravity-geoid-and?redirectedFrom=fulltext) studies, maximum depth of sensitivity for each degree of spherical harmonic is defined as Z<sub>max</sub>= r<sub>c</sub>/(n-1); r<sub>c</sub> is radius of earth, n is the degree of spherical harmonic and Z<sub>max</sub> is the maximum depth of sensitivity; On the other hand λ (Wavelength)=2πr<sub>c</sub>/n. Since this study aims to find Moho depth (depth of crust-mantle boundary), it can be said the desired depths are below 100 km, so there is a need to use a high pass filter to remove the effect of low frequencies which belong to deep masses, in other words to remove the influence of masses close to the mantle-core boundary and pass high frequencies. In the following figures, free air gravity anomaly and its derivatives in three directions after using a high pass filter with cut-off wavelength of 1000 km are shown. The X and Y derivatives were calculated in the spatial domain using a simple nine-point convolution filter and the Z derivative was computed in the frequency domain using Fast Fourier Transform (FFT).

</DIV>

{{< figure src="FA_mgal_1000km.png" title="High pass filtered free air gravity anomaly (The Zagros Zone); cut-off wavelength of 1000 km" numbered="true" lightbox="true" >}}

{{< figure src="dx_mgal_1000Km.png" title="The X derivative" numbered="true" lightbox="true" >}}

{{< figure src="dy_mgal_1000Km.png" title="The Y derivative" numbered="true" lightbox="true" >}}

{{< figure src="dz_mgal_1000Km.png" title="The Z derivative" numbered="true" lightbox="true" >}}


<DIV align="justify">

The Moho depth in the Structural Zones of Iran (Zagros Fold & Thrust Belt, Sanandaj-Sirjan Zone, Alborz, Central Domain, Kopeh Dagh) was estimated by Euler Deconvolution method for 15 km to 55 km window sizes and 0 to 2 structural indices. the best window size and structural index in the structural zones were determined by comparing depths from Euler Deconvolution method and those of seismic studies (receiver function method) in 14 seismic stations of the studied region, then the results were compared to CRUST2.0 model and other research works. In the Zagros zone, the results show that for a window size of 40-45 km and structural index of 0.5 the best Moho depth is estimated using Euler Deconvolution algorithm. The following figure shows the results of estimating Moho depth by Euler Deconvolution method for window sizes of 15 km to 55 km and structural index of 0.5 along AB profile in the Zagros zone.

</DIV>

{{< figure src="a.png" title="Topography map with seismic stations" numbered="true" lightbox="true" >}}
{{< figure src="b.png" title="Variation of Moho depth along AB profile in the Zagros Zone" numbered="true" lightbox="true" >}}

