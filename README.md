Standard solar models
=====================
In solar physics, we have certain models that we consider the "standard" models of the Sun.  
These are the basic models we turn to when answering questions about solar parameters, either in the interior or in the atmosphere.
Here, we do not imply that "standard" models are necessarily the "best", 
but rather they are the models we tend to turn to when we want a rough sense of the Sun's properties or to answer student questions, 
as they are well constructued and have been tested against data.
When you ask a solar physicist what model to turn to, these are the likeliest first answers.


For the interior, arguably the standard solar model is ["model S"](https://users-phys.au.dk/~jcd/solar_models/), 
while for the solar atmosphere arguably the standard model is the [AV08 model](https://iopscience.iop.org/article/10.1086/523671), 
which is an update of the classic "VAL" atmosphere model.  
These models are published and freely available.

This repository provides some basic tools, along with text file copies of the models, for reading in and plotting basic properties of the Sun.


Model S
-------

```
solar_structure.read_model_S_GONG_format()
solar_structure.read_model_S_limited_format()
```

Tools in this section read structure data based on "model S", as reported in

     "The current state of solar modeling",
     Christensen-Dalsgaard, J., Däppen, W., Ajukov, S. V., Anderson, E. R., Antia, H. M., Basu, S., Baturin, V. A., Berthomieu, G., Chaboyer, B., Chitre, S. M., Cox, A. N., Demarque, P., Donatowicz, J., Dziembowski, W. A., Gabriel, M., Gough, D. O., Guenther, D. B., Guzik, J. A., Harvey, J. W., Hill, F., Houdek, G., Iglesias, C. A., Kosovichev, A. G., Leibacher, J. W., Morel, P., Proffitt, C. R., Provost, J., Reiter, J., Rhodes Jr., E. J., Rogers, F. J., Roxburgh, I. W., Thompson, M. J., Ulrich, R. K., 1996,
     Science, 272, 1286 - 1292.

and as freely available at:

     https://users-phys.au.dk/~jcd/solar_models/


solar atmosphere
----------------

```
solar_structure.read_solar_atmosphere()
```

Tools in this section read solar atmosphere data based on:

     "Models of the solar chromosphere and transition region from SUMER and HRTS observations: formation of the extreme-ultraviolet spectrum of hydrogen, carbon, and oxygen",
     Avrett, E. H., Loeser, R., 2008,
     The Astrophysical Journal Supplement Series, 175, 229-276
     DOI 10.1086/523671
     https://iopscience.iop.org/article/10.1086/523671

This model is an updated verison of "VAL" model (Vernazza et. al, 1981), and here we read in a text file version of Table 26 from Avrett & Loeser (2008).  This text file is a lightly formatted version of the data available at:

     https://iopscience.iop.org/article/10.1086/523671/fulltext/tb26.html

Primary formatting changes were to turn the header row into comments and to remove the '...' after the numbered indices.

Vernazza, J. E., Avrett, E. H., & Loeser, R. 1981, ApJS, 45, 635 (VAL)
