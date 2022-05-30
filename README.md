# Estimate of the catalog completeness within the sky localizations of gravitational-wave events.

The code analyzes the gravitational-wave sky localization observed during the O1, O2 and O3a runs from the LIGO and Virgo Collaborations. In particular, we estimate the catalogue completeness within the credible volume provided in the final skymaps issued in the first and second GWTC (Gravitational-Wave Transient Catalog).
We used GLADE (v 2.4)  from **Vizier**.

**Vizier** provides the most complete library of published astronomical catalogues --tables and associated data- with verified and enriched data, accessible through multiple interfaces. Query tools allow the user to select relevant data tables and to extract and format records that match certain criteria. More than *21,000 catalogues* are currently available.

For more information http://vizier.u-strasbg.fr

To perform the analysis, we defined the function *completeness*, which takes the url of the skymap and returns useful parameters such as 
**name**, the credible volume within the 3-D credible region **vol**, the total luminosities of galaxies inside the volume, **lum_tot**, the apparent mean magnitudue of the galaxies **m_th**, the mean luminosity distance, **distmean**, which are subsequently used in other functions.

Below the graph obtained for the event GW170817 with the algorithm that was run on 50 events of the first three observational runs of HLV from GWTC\nobreakdash-2. 
In red the Schechter function is described as a function of luminosities and considering:
 - $\phi^* = 1.6\pm (0.3)\times 10^{-2} h^3 Mpc^3 $ ;
 - $L^{*}_{B} = 1.2 \pm 0.1 \times 10^{10} h^{-2} L_{B,\odot}$ ;
 - $\alpha= -1.07 \pm 0.07$.
The distributions of luminosity of the galaxies contained within the 90\% of credible volume have been plotted in blue, considering a shell of distance $d_\mathrm{L} \pm 3\sigma$ and galaxies from GLADE (v.2.4) catalogue.
The graphs give us at a glance an estimate of the completeness of the catalogue with respect to the probability region where the GW event is localised.

![GW170817_schechter](https://user-images.githubusercontent.com/91550119/170940355-faa29752-1698-4aa2-bb76-d8bfda2b1875.png)


In order to get a more complete picture, we identify the intersection area with the Galactic dust extinction and what percentage of the gravitational-wave sky location falls in it. 

In case of event GW170817 you get the following map .

![intersection](https://user-images.githubusercontent.com/91550119/170942693-c84b149d-29fb-4225-bc23-793aeef33214.png)


A summary table is also provided in which a "completeness coefficient" is determined for each gravitational-wave sky localization.
The *completeness coefficient* can be transmitted via the GCN alert system whenever a gravitational event is recorded, so that telescopes can have an estimate of the completeness in the localisation region in order to detect the host galaxies. But also may be useful to understand which regions of the sky are incomplete so as to promote campaigns to increase the completeness.

*Maria Lisa Brozzetti*, <marialisa.brozzetti@studenti.unipg.it> 

*Giuseppe Greco*, <giuseppe.greco@pg.infn.it> 

*Gergely Dalya*, <gergely.dalya@ugent.be>
