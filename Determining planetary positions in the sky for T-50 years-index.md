---
master_file: "[[@DeterminingPlanetaryPositions]]"
---
# Index for Determining planetary positions in the sky for T-50 years.pdf

arXiv:0910.2778v1 [astro-ph.IM] 15 Oct 2009
P R A Y A S c© Indian Association of Physics Teachers Students’ Journal of Physics
Determining planetary positions in the sky for ±50 years to an
accuracy of 1◦ with a calculator
Tanmay Singal1 and Ashok k. Singal2
1 II Year B.Sc. Physics-Maths, St. Xavier’s College, Ahmedabad, India. Email: tanmaysingal@gmail.com 2 A&A Division, Physical Research laboratory, Ahmedabad, India. Email: asingal@prl.res.in
Abstract. In this paper, we describe a very simple method to calculate the positions of the planets in the sky. The technique used enables us to calculate planetary positions to an accuracy of 1◦ for ±50 years from the starting epoch. Moreover, this involves very simple calculations and can be done using a calculator. All we need are the initial specifications of planetary orbits for some standard epoch and the time periods of their revolutions.
1. INTRODUCTION
The night-sky fascinates people. To be able to locate a planet in the night sky is something that thrills people. Since the planets move with respect to the background stars and continuously change their positions in the sky, locating them in the sky could appear be a non-trivial task. It is a general notion that calculating the planetary positions is a very tedious task, involving a lot of complicated mathematical equations and computer work. However, to be able to locate planets in the sky one does not really need very accurate positions. After all, Kepler’s laws, which describe planetary orbits reasonably well, are mathematically simple. Hence, one could use Kepler’s law to predict planetary positions in which mutual influence of planets is not considered. Thereby an accuracy of ∼ 1◦ in planetary positions would be achieved. In this project, we employ a very simple method to calculate the positions of the planets. The technique we use enables us to calculate planetary positions to an accuracy of 1◦ for ±50 years from the starting epoch. Moreover, this involves very simple calculations and can be done using a calculator. All we need are the initial specifications of planetary orbits for some standard epoch and their time periods of revolution. Although accurate planetary positions could be obtained easily from the internet, yet it is very instructive and much more satisfying to be able to calculate these ourselves, starting from basic principles and using a simple procedure. Our first step would be to calculate the positions of all the planets (including Earth) in their orbits around the Sun. We initially consider the planets to revolve around the Sun in uniform circular
1



Tanmay Singal and Ashok k. Singal
motions. Knowing their original positions for the starting epoch, we calculate their approximate positions for the intended epoch. As a consequence of this approximation there will be an error since the actual orbits are elliptical. To get more accurate positions, we require some corrections, which are derived in Appendix A. These corrections account for the elliptical motion. Knowing the positions of the planets around the Sun, we can then use simple co-ordinate geometry to transform their position with respect to an observer on Earth. Our task becomes simple since the orbits of all planets more or less lie in the same plane, viz. the ecliptic plane. In this project, we calculate the motion of naked-eye planets only, although the procedure can be applied equally well for the remaining planets also.
2. CELESTIAL CO-ORDINATES
All celestial bodies in the sky, including stars, planets, Sun, Moon and other objects, appear to lie on the surface of a giant sphere called the Celestial Sphere. Due to Earth’s eastward rotation around its axis, the celestial sphere appears to rotate westward around Earth in 24 hours. Infinitely extending
Figure 1. Celestial sphere showing the ecliptic co-ordinate system [5]
2



Planetary positions in the sky to 1◦ accuracy
the plane of Earth’s equator into space it appears to intersect the celestial sphere to form a circle, which is called the Celestial Equator. As Earth moves around the Sun - as seen from the Earth - Sun changes its position with respect to the background stars. The path that Sun takes on the celestial sphere is called the “Ecliptic”. The familiar Zodiac constellations are just divisions of the ecliptic into twelve parts. Since all other planets revolve around Sun in nearly the same plane, they also appear to move on the ecliptic. The celestial equator is inclined to the ecliptic by 23.5◦. The points of intersections of these two circles on the celestial sphere are called the “Vernal Equinox” and the “Autumnal Equinox”. The Vernal Equinox, also known as the Spring Equinox, is the point on the celestial sphere that the Sun passes through around 21st of March every year. In astronomy, an epoch is a moment in time for which celestial co-ordinates or orbital elements are specified, while a celestial co-ordinate system is a co-ordinate system for mapping positions in the sky. There are different celestial co-ordinate systems each using a co-ordinate grid projected on the celestial sphere. The co-ordinate systems differ only in their choice of the fundamental plane, which divides the sky into two equal hemispheres along a great circle . Each co-ordinate system is named for its choice of fundamental plane. The ecliptic co-ordinate system is a celestial co-ordinate system that uses the ecliptic for its fundamental plane. The longitudinal angle is called the ecliptic longitude or celestial longitude (denoted λ), measured eastwards from 0◦ to 360◦ from the vernal equinox. The latitudinal angle is called the ecliptic latitude or celestial latitude (denoted β), measured positive towards the north. This coordinate system is particularly useful for charting solar system objects. The Earth’s axis of rotation precesses around the ecliptic axis with a time period of about 25800 years. Due to this, the equinoxes shift westwards on the ecliptic. Due to the westward shift of the Vernal Equinox, which is the origin of the ecliptic co-ordinate system, the ecliptic longitude of the celestial bodies increases by an amount 360/258 ∼ 1.4◦ per century. Most planets, dwarf planets, and many small solar system bodies have orbits with small inclinations to the ecliptic plane, and therefore their ecliptic latitude β is always small. Due of the planets’ small deviation from the plane of the ecliptic, the ecliptic longitude may alone suffice to locate planets in the sky.
3. CALCULATING PLANETARY POSITIONS
3.1 HELIOCENTRIC CIRCULAR ORBIT
Here, we consider the planets to move around Sun in circular orbits with a uniform angular speed. The initial values of mean longitudes (λi) of the planets given in Table 1 are for 1st of January, 2000 A.D., 00:00 UT (adapted from [1]). In Table 1, we have also listed the period, T (days), of revolution of the planets [2]. Then, the mean angular speed is give by, ω0 = 360/T (◦/day). We denote the Mean Longitude of the planets in the imaginary circular orbit for subsequent dates as λ0.
3



Tanmay Singal and Ashok k. Singal
Table 1. Mean longitude λ0 on 01/01/2007, 00:00 UT from the initial value λi
Planet λi (◦) T (days) ω0 (◦/day) λ0 (◦) λe (◦) Error (◦) Mercury 250.2 87.969 4.09235 274.3 268.7 +5.6 Venus 181.2 224.701 1.60213 317.8 317.8 0.0 Earth 100.0 365.256 0.98561 100.2 100.2 0.0 Mars 355.2 686.980 0.52403 255.1 244.5 +10.6 Jupiter 34.3 4332.59 0.08309 246.8 242.6 +4.2 Saturn 50.1 10759.2 0.03346 135.7 140.2 -4.5
We now demonstrate how to calculate λ0 for Mars on 1st January 2007.
λi of Mars on 01.01.2000 at 00:00 UT = 355.2◦ . No. of days b/w 01.01.2000 and 01.01.2007 = 2557 days. Mean angle traversed duration this period = 0.52403 × 2557 = 1339.9◦. So, λ0 on 01.01.07 at 00:00 UT = 355.2 + 1339.9 = 255.1◦.1
In the same way, mean longitudes of all planets have been calculated in Table 1 for the same epoch. For a comparison, we have listed the actual longitude values (λe) from Indian Ephemeris [4] for that epoch. Here, we see, from the error in column 7, that one has to correct for the elliptical shape of the orbit, at least for some of the planets.
3.2 HELIOCENTRIC ELLIPTICAL ORBIT
Before we make corrections for the elliptical shape of the orbit we need to know the orientation of the ellipse within the ecliptic and that can be defined by the longitude of the perihelion.2 Longitudinal distance of the planet from the perihelion along the elliptical orbit is known as its Anomaly (denoted by θ), while angular distance of mean position of planet with respect to the perihelion is called the Mean Anomaly (denoted by θ0). As has been discussed in Appendix A, there is a one–to–one correspondence between θ and θ0. The correction ∆θ to be added to θ0 (Equation 4) is,
∆θ = 2 e sin θ0 + 5
4 e2 sin 2θ0
where e is the eccentricity of the ellipse.
1We have taken out the integer number of complete orbits. 2Perihelion is the point on the elliptical orbit closest to the Sun, while aphelion is the point farthest from Sun.
4



Planetary positions in the sky to 1◦ accuracy
Table 2. Corrected longitude λ on 01/01/2007, 00:00 UT
Planet λ0 (◦) λp (◦) θ0 (◦) e ∆θ (◦) θ (◦) λ (◦) λe (◦) Error (◦) Mercury 274.3 77.5 196.8 0.2056 -5.1 191.7 269.3 268.7 0.6 Venus 317.8 131.6 186.2 0.0068 -0.1 186.1 317.8 317.8 0.0 Earth 100.2 102.9 357.3 0.0167 -0.1 357.2 100.2 100.2 0.0 Mars 255.1 336.1 279.0 0.0934 -10.7 268.3 244.5 244.5 0.0 Jupiter 246.8 14.3 232.4 0.0485 -4.2 228.2 242.6 242.6 0.0 Saturn 135.7 93.1 42.6 0.0555 4.5 47.1 140.3 140.2 0.1
Let’s consider Mercury’s position on 01/01/07 at 00:00 UT.
Mean longitude, λ0 = 274.3◦ Perihelion Longitude, λp = 77.5◦ Mean anomaly, θ0 = λ0 − λp = 196.8◦
1st order correction, 2e sin θ0 = 2 × 0.2056 × sin(196.8◦) = −0.11885 rad = −6.8◦ 2nd order correction, 5
4 e2 sin 2θ0 = 1.25 × (0.2056)2 × sin(33.6◦) = 0.02924 rad = 1.7◦ ∆θ = (1st order correction) + (2nd order correction) = −6.8 + 1.7 = −5.1◦ Anomaly, θ = θ0 + ∆θ = 196.8 − 5.1 = 191.7◦
Precession of vernal equinox in 7 yrs = 7 × 360/25800 = 0.1◦. λ = λ0 + ∆θ + precession of vernal equinox = 274.3 − 5.1 + 0.10 = 269.3◦.
We can obtain corrections for the elliptical orbits of the remaining planets in the same way. In Table 2, We have listed values of the longitude of perihelion (λp) and eccentricity (e) for all planets, taken from [1]. Also tabulated are the calculated anomaly (θ) and longitude (λ). From Table 2, we see that the errors now are indeed smaller than 1◦.
3.3 GEOCENTRIC PERSPECTIVE
Until now, we have calculated the longitudes λ of the planets on the celestial sphere centered on the Sun. We can also calculate radii r of their orbits around the sun, giving their positions in polar form (r, λ). To get the positions of planets on the celestial sphere centered on the Earth, we convert the polar co-ordinates into rectangular form and after shifting the origin from Sun to Earth, we change them back into polar form. For converting into a rectangular form, we have to decide upon the direction of the X and Y axes. We assume X to be in the positive direction along the line joining the Sun to the Vernal Equinox, and Y to be perpendicular to X in the ecliptic plane in such a way that the longitude is a positive angle.
5



Tanmay Singal and Ashok k. Singal
3.4 AN EXAMPLE
As an example, this procedure is demonstrated for Mercury’s position on 01/01/07 at 00:00 UT.
1 HELIOCENTRIC CO-ORDINATES
Distance, r, of Mercury from Sun can be obtained from anomaly θ as,
r = a(1 − e2)
1 + e cos θ = 0.464A.U.,
where a = 0.387A.U. is the length of semi–major axis of its elliptical orbit. Thus heliocentric polar co-ordinates of Mercury are (0.464 A.U., 269.3◦). Then we can get heliocentric rectangular co-ordinates of Mercury as,
Xh = r cos(λ) = −0.006 A.U. Yh = r sin(λ) = −0.464 A.U.
Similarly we get heliocentric rectangular co-ordinates of Earth as,
X
0 = −0.174 A.U. Y
0 = 0.968 A.U.
2 GEOCENTRIC CO-ORDINATES
Geocentric rectangular co-ordinates of Mercury then are
Xg = Xh − X0 = 0.168 A.U. Yg = Yh − Y0 = −1.432 A.U.
Converting these into polar form, we get the geocentric distance and longitude as,
rg = √(X2
g +Y2
g ) = 1.442 A.U. λg = tan−1(Yg/Xg) = 276.7◦.
We give the calculated geocentric longitudes, on 01.01.07 at 00:00 UT, of various planets in Table 3. Comparing with the geocentric longitudes from ephemeris λge, it can be seen that the errors are much less than 1◦. In the Earth/Sun row in Table 3, rg, λg and λge are the geocentric values for the Sun’s position. The position of Sun on the celestial sphere, as seen from Earth, is in a direction exactly opposite to that of Earth as seen from the Sun. Therefore the geocentric longitude of Sun is the heliocentric longitude of Earth plus 180◦.
6



Planetary positions in the sky to 1◦ accuracy
Table 3. Geocentric longitude λg on 01/01/2007, 00:00 UT
Planet a (A.U.) e r (A.U.) λ (◦) rg (A.U.) λg (◦) λge (◦) Error (◦) Mercury 0.387 0.2056 0.464 269.3 1.44 276.7 276.5 0.2 Venus 0.723 0.0068 0.728 317.8 1.62 296.1 296.1 0.0 Earth/Sun 1.00 0.0167 0.983 100.2 0.983 280.2 280.2 0.0 Mars 1.52 0.0934 1.51 244.5 2.38 258.4 258.4 0.0 Jupiter 5.20 0.0485 5.36 242.6 6.17 248.2 248.2 0.0 Saturn 9.55 0.0555 9.17 140.3 8.45 144.6 144.5 0.1
We have ignored any perturbations on the motion of a planet due to the effect of other planets which may distort its elliptical path. We are able to get the accuracy of < 1◦ for long periods (±50 years) because most of the terms ignored in the heliocentric longitude calculations are periodic in nature and do not grow indefinitely with time (see e.g., [3]). The other parameters characterizing the elliptical orbit, like the longitude of the perihelion, semi–major axis and eccentricity etc. change so slowly with time that for the accuracy we are interested in, these can be considered constant for ±50 years.
4. LOCATING PLANETS IN THE SKY
Now that we have calculated the geocentric longitudes of the planets, we are in a position to locate them in the sky. Any one familiar with the Zodiac constellations could locate a planet from its position in the constellation in which it lies. The ecliptic is divided into 12 Zodiac signs – Aries, Taurus, Gemini, Cancer, Leo, Virgo, Libra, Scorpio, Sagittarius, Capricorn, Aquarius, Pisces. The Vernal equinox, at zero ecliptic longitude, is the start of the first Zodiac sign and is also known as the First Point of Aries. But there is a caveat attached. Because of the precession the vernal equinox has shifted westward by almost the full width of a constellation in the last ∼ 2000 years since when the Zodiac signs and constellation were perhaps first identified. As a consequence, the First Point of Aries now lies in the constellation Pisces. For example, on 01/01/2007, geocentric longitude 276.7◦ of Mercury implies it is in the 10th Zodiac sign Capricorn, but actually lies in the Sagittarius constellation, taking into account the shift by one constellation due to precession. There are further complications. The twelve constellations are not all of equal length of arc along the ecliptic longitude. Moreover there is another constellation, viz. Ophiuchus, through which the ecliptic passes. However these complications are somewhat set aside by the fact that there are only about half a dozen stars in the Zodiac with an apparent brilliance comparable to the naked–eye planets, therefore with some familiarity of the night-sky, one could locate the planets easily from their geocentric longitude values. It further helps to remember that unlike stars, the planets, because of their large angular sizes, do not twinkle. For a more precise location of a planet we can calculate its relative angular distance from the Sun along the ecliptic.
7



Tanmay Singal and Ashok k. Singal
Table 4. Elongations of the planets on 01/01/2007
Planet λe(◦) ψ(◦) Rise Time ψ(◦) Setting Time at 05:30 IST Before Sunrise at 17:30 IST After Sunset Sun 280.2 - - - Mercury 276.7 -3.5 0h14m -3.2 Venus 296.1 15.9 - 16.0 1h04m Mars 258.4 -21.8 1h27m -21.9 Jupiter 248.2 -32.0 2h08m -32.4 Saturn 144.6 -135.6 9h02m -136.2
The difference between the geocentric positions of a planet and Sun (Table 4) is called the elongation (ψ) of the planet and it tells us about planet’s position in the sky with respect to that of the Sun. The longitude increases eastwards, therefore, if the longitude of the planet is greater than that of the Sun, then the planet lies to the east of the Sun. That means, in the morning the Sun will rise before the planet but in the evening the planet will be setting after the Sun. So the planet will be visible in the evening sky in the west. On the other hand, if the geocentric longitude of the planet is smaller than that of the Sun, it will rise before the Sun and will be visible in the morning in the eastern sky.
Figure 2. A schematic representation of the elongations of planets at the times of sunrise and sunset on 1st January, 2007
8



Planetary positions in the sky to 1◦ accuracy
In Table 4, positions of planets with respect to Sun on 01.01.07 are given for 00:00 UT, which corresponds to 05:30 IST (Indian Standard Time). For example, the geocentric longitude of Mars with respect to Sun is 258.4 − 280.2 = −21.8◦. Thus Mars has a western elongation ∼ 22◦ on 01.01.07, 05:30 IST. As Earth completes a rotation in 24 hours, the westward motion of the sky is at a rate 15◦/ hour. This rate is strictly true for the celestial equator, but we can use this as an approximate rotation rate even for the ecliptic, which is inclined at a 23.5◦ to the equator. Therefore Mars will rise 22/15 ∼ about one and half hour before the Sun. We have also tabulated elongations of the planets for the same date but at 17:30 IST. Note that this corresponds to 12:00 UT and there is a change in the elongation values during this half a day due to shifts in the geocentric longitudes of the planets and the sun. Venus with an eastern elongation ∼ 16◦ on that evening, will be setting a little more than an hour after the sunset. This way, one can easily locate the planets in the sky from their elongations. Figure 2 is a schematic representation of the relative positions of the planets and the sun in the morning and evening of 1st January, 2007.
5. CONCLUSIONS
It is a general notion that calculation of position of planets in the night sky is a difficult job, which can be accomplished only by complex scientific computations, using fast computers. The motive of this project has been to bring out the fact that such complex and accurate computations are not always really necessary. One can calculate the position of planets using the method derived here and get the thrill of finding the planet at the predicted position in the night sky. We have been able to obtain the position of planets within an accuracy of 1◦, using a calculator. This method can be used to reckon planetary positions up to ±50 years of the starting epoch.
ACKNOWLEDGEMENTS
TS expresses his gratitude to the Astronomy and Astrophysics Division, and in particular Dr. Hari Om Vats, of the Physical Research laboratory Ahmedabad, where work on this project was done.
APPENDIX A: CORRECTION FOR THE ORBITAL ELLIPTICITY
We compute the correction for motion of a planet in an actual elliptical orbit from that in an imaginary circular orbit. Period of revolution in circular orbit is taken to be exactly the same as that in the elliptical orbit. The origin of the mean longitude in circular orbit is chosen such that λ0 coincides with the longitude λ of the planet when it is at the perihelion in its elliptical orbit. For mathematical convenience, we take t = 0 at that instant. Then λ0(0) = λ(0). Let λp be the longitude of the perihelion of the planet’s elliptical orbit. We subtract the λp from λ0 and λ to obtain what is called
9



Tanmay Singal and Ashok k. Singal
Figure 3. A schematic diagram of the planet in circular and elliptical motion
the “mean anomaly” and “anomaly” respectively (denoted here by θ0 and θ, respectively) of the planet. Then Mean Anomaly, θ0 = λ0 - λp, Anomaly, θ = λ - λp. Then θ0(0) = θ(0)
In circular motion, the angular speed of the planet is constant. However, in the elliptical motion, the angular speed of the planet is not constant. Let a time t has passed after t = 0. Then, the change in θ0 of the planet is ω0t whereas the change in θ of the planet won’t be the same because of the variation in the angular speed along elliptical trajectory.
Let ∆θ(t) = θ(t) - θ0(t).
We know that θ0(t) and θ(t) are periodic by the same time interval, T , as T is the time period of revolution in both the cases (elliptical and circular motion). Hence, all value of θ0(t) and θ(t) repeat after a time period of T. Hence, θ0(t) and θ(t) have a one–to–one relation. Hence, ∆θ also repeats after time T . The uniform circular motion thus is a useful approximation because the error ∆θ is periodic with time and does not keep accumulating with time to grow to very large values. To find the correction, first consider an elliptical orbit of a planet around the Sun as shown in Figure 3. We use the equation of the ellipse in polar co-ordinates (r, θ) where θ is the anomaly. The equation of the ellipse then is,
10



Planetary positions in the sky to 1◦ accuracy
r= l
1 + e cos θ = a(1 − e2)
1 + e cos θ (1)
where l = a(1 − e2) is the semi–latus rectum with a as the semi–major axis and e the eccentricity of the ellipse. The semi–minor axis of the ellipse is b = a√(1 − e2). Now, total area of the ellipse A = πab is swept in T , the time period of revolution. From Kepler’s second law we know that the rate of area swept out by the position vector of planet (with respect to Sun) is a constant. Therefore the rate of area swept is,
dA
dt = r2
2
dθ
dt = πab
T
Substituting from Equation (1), we get
2π
T = (1 − e2) 3
2
(1 + e cos θ)2
dθ dt
We notice that 2π/T is nothing but the mean angular speed ω0. Therefore
θ
0(t) =
∫t
0
ω
0 dt =
∫t
0
(1 − e2) 3
2
(1 + e cos θ)2 dθ (2)
We want to get the equation in the form, θ = θ0 + ∆θ, so that by adding the longitude of the perihelion on both sides of the equation, we could get the relation between the correct longitude λ and the mean longitude λ0. A direct integration of Equation (2) may be very complicated. But we can expand the integrand as a series and integrate only a few first most significant terms. A binomial series expansion is possible because the eccentricity of an ellipse, e < 1. Also, during the expansion we drop terms of order e3 or higher.
θ
0(t) =
∫t
0
(1 − 3
2 e2 + · · ·)(1 − 2 e cos θ + 3 e2 cos2 θ · · ·) dθ
After integration we get,
θ
0 = θ − 2 e sin θ + 3
4 e2 sin 2θ + · · ·
which can be written as
∆θ = θ − θ0 = 2 e sin θ − 3
4 e2 sin 2θ + · · · (3)
However we want the r.h.s. of Equation (3) to be expressed in terms of θ0. For that we can substitute θ = θ0 + ∆θ on the r.h.s. to get,
∆θ = 2 e sin(θ0 + ∆θ) − 3
4 e2 sin[2(θ0 + ∆θ)] + · · ·
11



Tanmay Singal and Ashok k. Singal
Expanding in powers of ∆θ and neglecting terms of order e (∆θ)2, e2 ∆θ and higher we get,
∆θ (1 − 2 e cos θ0) = (2 e sin θ0 − 3
4 e2 sin 2θ0),
or
∆θ = (2 e sin θ0 − 3
4 e2 sin 2θ0) (1 − 2 e cos θ0)−1.
Again Expanding in powers of e and ignoring terms of order e3 or higher, we get,
∆θ = 2 e sin θ0 + 5
4 e2 sin 2θ0 (4)
which is the required correction term.
APPENDIX B: POSITION OF THE MOON
Here we determine Moon’s position for any given epoch, say, 1st January 2007, 00 UT, starting from the initial epoch 1st January 2000, 00 UT. Moon moves in a geocentric orbit of mean eccentricity e = 0.0549 and a tropical revolution period of T = 27.32158 days, corresponding to a mean angular speed ω0 = 13.17640◦/day with respect to the vernal equinox. From the initial value λi = 211.7◦, Moon’s mean longitude is calculated as, λ
0 = 211.7 + 13.17640 × 2557 = 63.8◦.
But before we correct for the ellipticity of the Moon’s orbit, we need to consider that unlike in a planetary orbit where the position of the perihelion change so slowly with time that it can be considered constant for ±50 years, in Moon’s orbit the perigee rotates forward with respect to the vernal equinox with a period of 3231.4 days (∼ 8.85 years), corresponding to an angular speed 0.11141◦/day. With an initial value of 83.3◦, the longitude of the perigee, on January 1, 2007, 00:00 UT is then given by, λp = 83.3 + 0.11141 × 2557 = 8.2◦.
From this we get Moon’s mean anomaly for a circular motion as, θ0 = λ0 − λp = 55.6◦. We can now use Equation (4) in the same way as for the planets to get the correction for the ellipticity ∆θ = 5.4◦, which gives λ = λ0 + ∆θ = 69.2◦. However, the value obtained thus is accurate only up to ∼ 2◦. The reason being that there is an important perturbation term, known as Evection, which depends upon Moon’s mean elongation ψ0 as well as its mean anomaly θ0, and has a value, ∆θev = 1.27◦ sin(2ψ0 − θ0). Substituting for ψ0 = 63.8 − 280.2 + 360.0 = 143.6◦, we get, ∆θev = 1.27 sin(2 × 143.6 − 55.6) = −1.1◦.
Thus Moon’s corrected longitude on 1st January, 2007, 00:00 UT is λ = 69.2 − 1.1 = 68.1◦, and the elongation ψ calculated thence is 147.9◦, well within a degree of the ephemeris values of 67.4 and 147.2◦ respectively. There is another feature of the Moon’s motion which has a direct bearing on the time of occurrences of solar and lunar eclipses. Moon’s orbit is inclined to the ecliptic with a mean inclination of 5.16◦, intersecting it at points known as the ascending and descending nodes. The ascending node
12



Planetary positions in the sky to 1◦ accuracy
is the one where Moon crosses the ecliptic in a northward direction. Gravitational pull of the Sun causes a precession of the axis of Moon’s orbital plane around that of the ecliptic with a tropical period of 6798.4 days (∼ 18.6 years). Consequently the nodes of the Moon’s orbit have a retrograde motion of ∼ 0.05295◦/day around the ecliptic. With an initial value of 125.1◦ on 1st January 2000, 00 UT, the longitude of the ascending node for the epoch January 1, 2007, 00:00 UT is given by, Ω = 125.1 − 0.05295 × 2557 = −10.3◦, i.e., 349.7◦, while the descending node is 180◦ away at 169.7◦.
A solar or lunar eclipse can only occur when Sun’s longitude is close to that of one of the nodes and the Moon’s elongation is either ∼ 0◦ (solar eclipse) or ∼ 180◦ (lunar eclipse).
APPENDIX C: THE ASTRONOMICAL CALENDAR
In all the examples presented above, the calculations were made using a scientific calculator. This procedure is appropriate for quickly getting some occasional planetary positions while locating these objects in the sky. However if one wants to do many computations, say calculate positions for all planets for each day of the year, the process becomes tedious and the chances of a numerical mistake occurring in manual calculations become high. Since the process of computing planetary positions is a repetitive one, it could then be much more convenient to write a simple computer programme using the algorithm described above to carry out the calculations. We have written such a programme to compute positions of all the planets as well as of the Moon for each day of a specified year and present the results in the form of an astronomical calendar which gives elongations of different planets for all days of that particular year. The calendar allows us to locate the naked-eye planets in the sky for any time of the corresponding year. The horizontal axis displays the elongation in hours (one hour corresponds to 15◦), and is centred around the Sun, which by definition has a zero elongation. The vertical axis marks the day of the year. Thus to locate a planet on any given date of the year, we select that date on the vertical axis and then move in a horizontal direction till we find the planet. From the elongation of the planet we can easily locate it in the sky. We can use the calendar to find what all planets are above the horizon at any time of the day. Suppose for a given date of the year we want to locate all planets visible in the sky at, say, dawn. The Sun, at 0h elongation, will at that time be just rising near the eastern horizon and the −12h elongation point in the calendar will be near the western horizon. The intermediate elongation points will be at in-between positions on the celestial hemisphere, e.g., the −6h elongation point will be close to the culmination point (the point nearest to the zenith). This way going along the horizontal direction from 0h to −12h at the chosen date, we will find the celestial position of all planets visible in the morning sky on that date. At dusk, with sun setting near the western horizon, the visible sky will stretch eastward from 0h to 12h elongation on the calendar. Similarly one can locate planets on the celestial sphere at other hours of the time. At midnight, with culmination point being at 12h (which is the same as −12h), the sky towards west will stretch from 12h to 6h and that towards east will be from −12h to −6h elongation, while at 9 p.m., with the culmination point at
13



Tanmay Singal and Ashok k. Singal
Figure 4. Astronomical calendar for locating planets in the sky for the year 2010
9h, the celestial hemisphere will stretch west to east between 3h and −9h elongations. The slant dotted lines running across the calendar from west to east almost every month represent Moon’s path. Their dates of intersection with the Sun’s path at 0h elongation mean new Moon days, while intersections with the midnight line (at ±12h elongation) imply full Moon days, with the intermediate phases at the in-between dates. The faint lines in the calendar represent the relative positions of the ascending and descending nodes of Moon’s orbital plane. Intersection of the sun’s path (at 0h elongation) or of the midnight line (at ±12h) with one of the lines of nodes, indicate the possibility of occurrence of an eclipse. In the neighbourhood of these intersection points, at the time of a new moon there might possibly occur a solar eclipse while at the full moon time there is a possibility of a lunar eclipse. From the astronomical calendar for the year 2010, shown in Figure 4, we see that close to the intersection point of Sun’s path with the ascending node there is new Moon around 15th of January, which could thus be a solar eclipse. Actually because of the limited resolution of the display, the calendar can only be used as a quick indicator. For a better accuracy, one should go back to the actual tabulated data from which the calendar has been generated. From our computed data for the longitudes of the Sun, Moon and the lines of nodes for the year 2010, we find that the possible dates for the solar eclipses in the year 2010 are 15th January and 11th July, while lunar eclipses may occur on 26th June and 21st of December. From NASA’s eclipse web site [6] we find that there indeed are four eclipses in the year 2010 on these very dates.
14



Planetary positions in the sky to 1◦ accuracy
References
[1] Fr ̈anz M. and Harper D., Planetary and Space Science 50, 217 (2002)
[2] Nicholson I., “Unfolding Our Universe”, Cambridge University Press (1999)
[3] Simon J. L. et al, Astronomy Astrophysics 282, 663 (1994)
[4] “The Indian Astronomical Ephemeris for the year 2007”, The Indian Meteorological Department, Kolkata (2007)
[5] http://www.hps.cam.ac.uk/starry/mathtechniqueslrg.jpg
[6] http://eclipse.gsfc.nasa.gov/eclipse.html
15