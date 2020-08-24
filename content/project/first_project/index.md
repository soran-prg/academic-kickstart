---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Depth of the Moho Discontinuity from Parker-Oldenburg Inversion and Geopotential Models"
summary: ""
authors: []
tags: [Moho Depth]
categories: []
date: 2020-01-09T16:34:05+03:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "featured.jpg"
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
The Parker-Oldenburg inversion algorithm is defined as follows:

$$h(x)=F^{-1}(\frac{-F[\Delta g(x)]e^{-kz_0}}{2\pi G \rho}-\displaystyle\sum_{n=2}^{\infty} \frac{k^{n-1}}{n!}F[h^{n}(x)])$$

<DIV align="justify">
Where F is the Fourier transform operator; ∆g(x) is gravity anomaly; h(x) is the depth to the interface; k is the wavenumber; G is the gravitational constant; ρ is the density contrast across the interface; and z<sub>0</sub> is the average depth of the horizontal interface. According to this algorithm, the topography of the interface density can be estimated by an iterative inversion procedure. The first approximation of the topography interface is computed by assigning h(x)=0. Iteratively, the value of h(x) is used in the equation to calculate a new estimate of h(x) until a reasonable solution is acquired. Due to the fact that the Parker-Oldenburg inversion method is unstable at high frequencies, a cosine low pass filter is utilized for constraining high frequency signals and series convergence. The high-cut filter (HCF) is defined as follows (WH and SH are the cut-off frequencies):
</DIV>

$$HCF(k)=\frac{1}{2}[1+\cos(\frac{k-2\pi \times WH}{2 \times (SH-WH)})] \ \ for \ \    WH \lt k \lt SH$$

$$HCF(k)=0 \ \ for \ \ k \gt SH$$

$$HCF(k)=1 \  \ for \ \ k \lt WH$$


<DIV align="justify">
It should be noted that when the difference between two successive approximations is lower than a convergence criterion or when a certain number of iterations is obtained, the iterative procedure will be terminated. In this study, the complete Bouguer gravity anomaly has been computed from the EGM2008 global geopotential model and ETOPO1 elevation data.
</DIV>

$$\Delta g_ {CB} = \Delta g_ {FA} - C_ {sb} +T.C.$$

<DIV align="justify">

Where ∆g<sub>CB</sub> is the complete Bouguer gravity anomaly; ∆g<sub>FA</sub> is the Free-Air gravity anomaly that is calculated from the spherical harmonics of the EGM2008 geopotential model up to degree and order of 2190; C<sub>sb</sub> is the simple Bouguer reduction that is defined as C<sub>sb</sub>=2.π.ρ.G.H<sup>o</sup> (ρ: 2670kg/m<sup>3</sup>; G: gravitational constant; H<sup>o</sup>: orthometric elevation acquired from ETOPO1 model); and T.C. is the terrain effects.
                      
                      
The computed Bouguer anomaly is a combination of long- and short-wavelength features. Generally speaking, a deeper source produces gravity anomalies with longer wavelength than a shallower source with the same size and density. In this study, in order to distinguish between deeper and shallower sources and do away with Bouguer anomalies with short wavelengths associated with shallow crustal sources, the radially averaged power spectrum of the complete Bouguer data has been calculated by Fourier analysis. Considering the log of power of the Bouguer gravity spectrum as a function of wavenumber, the mean depth of the interfaces is estimated by the power spectrum analysis. According to the plot of logarithm of the spectral energy against wavenumber, the spectral energy decays as the wavenumber increases. Mainly, this decay process is controlled by the ensemble average depth of the random distribution of sources, which can be predicted by detecting the linear trends of the plot and fitting a linear function to each segment concerning residual or regional anomalies. The mean depth of the interfaces equals the half of the slope of the segments ([Spector & Grant (1970)](https://pubs.geoscienceworld.org/geophysics/article-abstract/35/2/293/71153/Statistical-models-for-interpreting-aeromagnetic?redirectedFrom=fulltext)). The reference level (z<sub>0</sub>) for the Parker-Oldenburg inversion approach and cut-off wavelengths for differentiating the regional complete Bouguer anomaly (high wavelength anomalies corresponding to deep sources), which is utilized for the Moho depth estimation, from the residual one (short wavelength anomalies relating to shallow sources) have been derived from the power spectral analysis results. The density contrast between upper mantle and lower crust was computed from CRUST 1.0 and CRUST 2.0 models. 

</DIV>

{{< figure src="hhbhb.jpg" title="Radially averaged power spectrum of the complete Bouguer anomaly, three linear trends corresponding to causative sources at mean depths of 91.7, 23.93, and 6.09 km" numbered="true" lightbox="true" >}}

{{< figure src="jij.jpg" title="The complete Bouguer anomaly map on the Kopeh Dagh structural zone, northeastern Iran" numbered="true" lightbox="true" >}}

{{< figure src="huuuh.jpg" title="Topography from ETOPO1" numbered="true" lightbox="true" >}}

{{< figure src="ghg.jpg" title="Density contrast between the upper mantle and lower crust calculated from CRUST 1.0 model" numbered="true" lightbox="true" >}}

{{< figure src="featured.jpg" title="Depth of the Moho discontinuity from the Parker-Oldenburg inversion algorithm" numbered="true" lightbox="true" >}}

{{< figure src="ppp1.jpg" title="Moho depth variation along profile AB" numbered="true" lightbox="true" >}}

{{< figure src="ppp2.jpg" title="Moho depth variation along profile CD" numbered="true" lightbox="true" >}}
